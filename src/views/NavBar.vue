<template>
  <v-navigation-drawer expand-on-hover rail>
    <v-divider></v-divider>

    <v-list density="compact" nav>
      <v-list-item prepend-icon="mdi-home" title="Home" :to="'/'"></v-list-item>
      <v-list-item prepend-icon="mdi-folder" title="Dosen" :to="'/dosen'"></v-list-item>
      <v-list-item prepend-icon="mdi-folder" title="Mahasiswa" :to="'/mahasiswa'"></v-list-item>
      <v-list-item prepend-icon="mdi-folder" title="Ruangan" :to="'/ruangan'"></v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>
