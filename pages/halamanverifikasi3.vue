<template>
    <v-container>
        <v-btn icon>
            <v-icon>mdi-close</v-icon>
        </v-btn>
        <v-flex class="text-center mt-7">
            <img width="250" src="https://s3-alpha-sig.figma.com/img/5556/7bee/cf82a33ebcf83dbc31731e227315c8ae?Expires=1598832000&Signature=aJDuv1NKvOnIy6apHtGJR0Blx5XDanMfIhfj4tL3n5fF4TO82AMSd8r~FG-zybCJ4VTOQAua0FeKr5gJC~SzrlHVemqAtPt6FwGdgKzUmhkrPEP04966ZehumV9oN-Uzlo88N5Jx9g53abN6SFar1oSi6rsT79l5~hBH2hKutMUz2mD5qThWT6d7yRChViyKFvBqCriQrOdULX7fcbZ6wJvMtORp3J1hCYkChQ0rANPgkDH7nIkkTklFAnzOIywFKXj4BdeFMu5~NbMq2HxdfGhn6SJPgVZAH6vMAOo3-rTCcIpryrGIurYDHvc12zcO4sBo5knsKaS-2KMqjmHuOw__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            <h3 class="orange--text mt-3">Langkah Kedua</h3>
            <h5 class="mt-3">Foto diri / Selfie beserta KTP.<br>Selfie dengan KTP ya, bukan istri, pacar, apalagi mantan.
            Pastikan juga foto diri berserta KTP difoto secara langsung dari kamera, bukan hasil screenshoot atau tangkapan layar.
            </h5>
        </v-flex>
        <v-flex class="text-center mt-3">
            <v-btn
                x-large
                elevation="3"
                rounded 
                class="orange accent" 
                @click="onPickFile">   
                <v-icon class="mr-1">mdi-camera</v-icon>
                Upload Foto
            </v-btn>
            <input 
                type="file" 
                style="display: none" 
                ref="fileInput" 
                accept="image/*"
                @change="onFilePicked">
        </v-flex>
        <v-flex class="text-center mt-2">
            <img :src="imageUrl" height="180">
            <h5>Pastikan foto wajah dan KTP terlihat jelas, dan pastikan juga agar informasi KTP di dalam foto bisa dibaca.</h5>
        </v-flex>
        <div class="text-center">
            <n-link to="halamanverifikasi4" class="text-decoration-none">
                <v-btn class="mt-5" large color="orange" outlined rounded elevation="3">
                    Konfirmasi Dokumen
                </v-btn>
            </n-link>
        </div>
    </v-container>
</template>
<script>
export default {
    data() {
        return {
            imageUrl: '',
            image: null
        }
    },
    methods : {
        onPickFile() {
            this.$refs.fileInput.click();
        },
        onFilePicked (event) {
            const files = event.target.files
            let filename = files[0].name;
            if (filename.lastIndexOf('.') <= 0) {
                return alert('Silahkan Upload File yang Valid!')
            }
            const fileReader = new FileReader;
            fileReader.addEventListener('load', () => {
                this.imageUrl = fileReader.result
            })
            fileReader.readAsDataURL(files[0])
            this.image = files[0]
        }
    }
}
</script>