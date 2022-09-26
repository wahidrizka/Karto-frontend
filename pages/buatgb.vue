<template>
    <div>
        <v-toolbar short dense block>
            <n-link to="/" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-close</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Galang Bantuan</h5>
            </v-toolbar-title>
        </v-toolbar>
        <v-stepper v-model="galangbantuan">
            <v-stepper-header>
                <v-stepper-step :complete="galangbantuan > 1" step="1"></v-stepper-step>
                <v-divider></v-divider>
                <v-stepper-step :complete="galangbantuan > 2" step="2"></v-stepper-step>
                <v-divider></v-divider>
                <v-stepper-step step="3"></v-stepper-step>
            </v-stepper-header>
            <v-stepper-items>
                    <v-stepper-content step="1">
                        <v-card-text>
                            <p>Halaman 1 dari 3</p>
                        </v-card-text>
                        <h4>Judul Galang Bantuan</h4>
                            <v-text-field
                                label="Masukan Judul Galang Bantuan" 
                                dense 
                                outlined 
                                single-line>
                            </v-text-field>
                        <h4>Kategori Galang Bantuan</h4>
                        <v-combobox
                            single-line 
                            clearable 
                            dense 
                            outlined 
                            v-model="kategorigb" 
                            :items="kategori" 
                            label="Pilih Kategori">
                        </v-combobox>
                        <h4>Bantuan yang Diperlukan</h4>
                        <v-combobox
                            single-line 
                            clearable 
                            dense 
                            outlined 
                            v-model="bentuk" 
                            :items="bentukbantuan" 
                            label="Pilih Bentuk Bantuan">
                        </v-combobox>
                        <h4>Target Banyaknya Bantuan</h4>
                        <v-text-field
                            prefix="Rp."
                            label="0" 
                            dense 
                            outlined 
                            single-line>
                        </v-text-field>
                        <h4>Tenggat Waktu Penggalangan Bantuan</h4>
                        <v-menu 
                            ref="menu" 
                            v-model="menu" 
                            :close-on-content-click="false" 
                            :return-value.sync="date"
                            transition="scale-transition" 
                            offset-y min-width="290px">
                            <template v-slot:activator="{ on, attrs }">
                                <v-text-field
                                    append-icon="mdi-calendar"
                                    v-model="date" 
                                    label="Pilih Tenggat Waktu Penggalangan" 
                                    readonly 
                                    v-bind="attrs" v-on="on"
                                    dense
                                    outlined
                                    single-line>
                                </v-text-field>
                            </template>
                            <v-date-picker
                                color="blue accent" 
                                header-color="orange"  
                                v-model="date" 
                                scrollable
                                locale="in-ID">
                                <v-spacer></v-spacer>
                                <v-btn color="blue accent" @click="menu = false">Batalkan</v-btn>
                                <v-btn color="blue accent" @click="$refs.menu.save(date)">Oke</v-btn>
                            </v-date-picker>
                        </v-menu>
                        <div class="text-right">
                            <v-btn color="blue accent" @click="galangbantuan = 2">
                                Selanjutnya
                            </v-btn>
                        </div>
                    </v-stepper-content>
                    <v-stepper-content step="2">
                        <v-card-text>
                            <p>Halaman 2 dari 3</p>
                        </v-card-text>
                            <h4>Deskripsi Penggalangan Bantuan</h4>
                            <v-textarea 
                                label="Ceritakan Alasan Penggalangan Bantuan Ini" 
                                dense 
                                outlined 
                                single-line>
                            </v-textarea>
                            <h4>Alamat Penerima Bantuan</h4>
                            <v-text-field
                                append-icon="mdi-crosshairs-gps"
                                label="Masukan Alamat Penerima Bantuan" 
                                dense 
                                outlined 
                                single-line>
                            </v-text-field>
                            <h4>Untuk Siapa Penggalangan Ini Ditujukan</h4>
                            <v-combobox
                                single-line 
                                clearable 
                                dense 
                                outlined 
                                v-model="penerimabantuan" 
                                :items="penerima" 
                                label="Pilih Untuk Siapa Penggalangan Ini">
                            </v-combobox>
                        <div class="d-flex justify-space-around">
                            <v-btn color="grey accent" @click="galangbantuan = 1">
                                Sebelumnya
                            </v-btn>
                            <v-btn color="blue accent" @click="galangbantuan = 3">
                                Selanjutnya
                            </v-btn>
                        </div>
                    </v-stepper-content>
                    <v-stepper-content step="3">
                        <v-card-text>
                            <p>Halaman 3 dari 3</p>
                        </v-card-text>
                        <h4>Bukti Untuk Memperkuat Penggalangan</h4>
                        <v-file-input
                            multiple 
                            v-model="files"
                            prepend-icon="mdi-image-outline"
                            single-line 
                            clearable 
                            dense 
                            outlined 
                            placeholder="Upload Foto Bukti"
                            :show-size="1000">
                            <template v-slot:selection="{ index, text }">
                            <v-chip
                                v-if="index < 2"
                                color="orange"
                                label>
                                {{ text }}
                            </v-chip>
                            <span
                                v-else-if="index === 2"
                                class="overline grey--text text--darken-3 mx-2">
                                +{{ files.length - 2 }} File(s)
                            </span>
                            </template>
                        </v-file-input>
                        <h4>Nomor Telepon yang Dapat di Hubungi</h4>
                        <v-text-field
                            hint="Utamakan Nomor Whatsapp"
                            persistent-hint
                            label="08XXXXXXXXXX" 
                            dense 
                            outlined 
                            single-line>
                        </v-text-field>
                        <v-checkbox class="mb-3"
                            v-model="checkbox"
                            :rules="[v => !!v || 'Setuju Untuk Melanjutkan']"
                            required>
                            <template v-slot:label>
                                <p class="text-caption text-justify mb-1"><b>Saya Setuju dangan <u>Syarat &
                                    Ketentuan</u> di Karto.id.</b> Anda juga menjamin kebenaran dari informasi yang diberikan dan
                                    menyetujui untuk <b>patuh</b> dengan segala ketentuan,
                                    tindakan dan keputusan dari <b>Karto.id.</b>
                                </p>
                            </template>
                        </v-checkbox>
                        <div class="d-flex justify-space-around">
                            <v-btn color="grey accent" @click="galangbantuan = 2">
                                Sebelumnya
                            </v-btn>
                            <v-btn color="blue accent" @click="galangbantuan = 3">
                                Selesai
                            </v-btn>
                        </div>
                    </v-stepper-content>
                </v-stepper-items>
        </v-stepper>
    </div>
</template>
<script>
    export default {
        data () {
            return {
                galangbantuan: 1,
                kategori: [
                    'Bencana Alam',
                    'Beasiswa Pendidikan',
                    'Bantuan Medis',
                    'Produk Inovasi',
                    'Bantuan Hukum',
                    'Tenaga Kerja',
                    'Lingkungan',
                    'Olahraga',
                    'Perdamaian & Toleransi',
                    'Pertanian',
                    'Kesejahteraan Hewan',
                    'Seni & Budaya'
                ],
                bentukbantuan: [
                    'Uang',
                    'Daging',
                    'Obat',
                    'Beras',
                    'Lainnya'
                ],
                penerima: [
                    'Saya Sendiri',
                    'Keluarga / Kerabat',
                    'Teman / Sahabat',
                    'Tetangga / Orang di Sekitar',
                    'Lembaga / Organisasi'
                ],
                files:[]
            }
        },
    }
</script>