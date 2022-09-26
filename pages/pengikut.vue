<template>
    <div>
        <v-toolbar dense>
            <n-link to="/profile" class="text-decoration-none">
                <v-icon>mdi-arrow-left</v-icon>
            </n-link>
            <v-toolbar-title class="ml-3">
                <h5>Pengikut</h5>
            </v-toolbar-title>
        </v-toolbar>
        <v-container>
            <div class="d-flex my-5" v-for="i in 12" :key="i">
                <div>
                    <v-avatar size="62" color="primary">
                        <img src="https://i.pinimg.com/originals/fc/fa/1d/fcfa1d4b4edede1f877ed78f697631cf.png">
                    </v-avatar>
                </div>
                <div class="ml-5 mt-1">
                    <h3>User{{i}}</h3>
                    <p class="font-weight-light">anonim0{{i}}</p>
                </div>
                <div>
                    <v-icon class="ml-3" color="blue lighten-1" >mdi-check-circle</v-icon>
                </div>
            </div>
        </v-container>
    </div>
</template>
