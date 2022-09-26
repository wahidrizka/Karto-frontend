<template>
    <div>
        <v-toolbar short>
            <n-link to="/kabarterbaru" class="text-decoration-none">
                <v-btn icon>
                    <v-icon>mdi-arrow-left</v-icon>
                </v-btn>
            </n-link>
            <v-toolbar-title>
                <h5>Kaori Menderita Kanker Stadium 3</h5>
            </v-toolbar-title>
        </v-toolbar>
        <v-container>
            <div class="ml-3 mt-5 d-flex">
                <v-avatar size="62">
                    <v-img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg"></v-img>
                </v-avatar>
                <div class="flex-column ml-3">
                    <h4 class="mb-1">MoriNana<v-icon color="primary" small class="mb-1 ml-2 mr-5">mdi-check-circle</v-icon></h4>
                    <p class="font-weight-light">nanamori</p>
                </div>
            </div>
            <v-flex class="text-center">
                <img :src="imageUrl" height="180">
            </v-flex>
            <div>
                <v-textarea
                    outlined
                    single-line
                    label="Post kabar terbaru"
                >
                </v-textarea>
                <v-flex class="text-center">
                    <v-btn
                        elevation="3"
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
            </div>
        </v-container>
        <v-btn block tile color="orange accent">Posting</v-btn>
    </div>
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