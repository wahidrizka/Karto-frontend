<template>
<div>
    <v-toolbar short>
        <n-link to="/profile" class="text-decoration-none">
            <v-btn icon>
                <v-icon>mdi-arrow-left</v-icon>
            </v-btn>
            </n-link>
        <v-toolbar-title>Edit Profil</v-toolbar-title>
    </v-toolbar>
    <div class="text-center ma-3">
        <v-avatar size="170">
            <img src="https://marucco-lino.com/wp-content/uploads/2019/06/%E6%A3%AE%E4%B8%83%E8%8F%9C.jpg">
        </v-avatar>
        <n-link to="#" class="text-decoration-none">
            <h3>Ganti Foto Profil</h3>
        </n-link>
        <div class="mt-3">
            <v-text-field dense v-model="name" label="Nama" outlined></v-text-field>
            <v-text-field dense v-model="username" label="Nama Pengguna" outlined></v-text-field>
            <v-text-field dense v-model="location" label="Lokasi" outlined></v-text-field>
            <v-text-field dense v-model="blog" label="Blog" outlined></v-text-field>
            <v-textarea v-model="bio" label="Bio" outlined></v-textarea>
            <v-btn color="primary">Perbarui</v-btn>
        </div>
    </div>
</div>
</template>

<script>
    export default {
        data: () => ({
            name: 'MoriNana',
            username: 'nanamori',
            location: 'Batikan, Juwiring',
            blog: 'morina.moe',
            bio: 'Sesungguhnya Harta Hanyalah Titipan Dari Allah SWT.'
        }),
    }
</script>