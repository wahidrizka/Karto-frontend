<template>
    <v-container>
        <v-btn icon>
            <v-icon>mdi-close</v-icon>
        </v-btn>
        <v-flex class="text-center mt-7">
            <img width="330" src="https://s3-alpha-sig.figma.com/img/11dd/ef0e/5e9abbbeed22c47d0ab46dad9db0e905?Expires=1598832000&Signature=WEK9cjyw3XM6iauHc2wZK~1031Odzq73wz96yXVQeEoeql9Jnv6~NanyZNemCFD7xnrVD~mJ7R4KrMipKb8icsoDEL2LXT3mWQjVVFhLmlTb3SFxwN5FaXs-FFpvj4ejt9RUtabau95X7UFutUAUy2rMzZBrLgMOqrDweUBf12tnUoRdQyRmckpZz2xV6i3W8voUd1YiMmkqLvHhsLrfHQRmOqixCDjptQtTfQxRNCKvoeEgSrKuyXopFowo-vcRg9e29k6KYa957fLlr93r9-ChDt~gImpwHPjyAbAFDM9W7H1a0B9XQ6IN7y92PyOkmEZd~RlKUxJ~JzgRShwAAQ__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA">
            <h3 class="orange--text mt-3">Langkah Pertama</h3>
            <h5 class="mt-3">Foto KTP.<br>Pastikan foto KTP yang masih berlaku dan asli, diambil dari kamera langsung, bukan hasil fotokopi, scan atau screenshoot.</h5>
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
            <h5>Pastikan foto KTP terlihat jelas, dan pastikan juga agar informasi KTP di dalam foto bisa dibaca.</h5>
        </v-flex>
        <div class="text-center">
            <n-link to="/halamanverifikasi3" class="text-decoration-none">
                <v-btn class="mt-5" large color="orange" outlined rounded elevation="3">
                    Langkah Selanjutnya
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