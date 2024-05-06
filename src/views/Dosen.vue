<template>
  <v-container>
    <v-row>
      <v-text-field label="NIDN" variant="outlined" v-model="dos.nidn"></v-text-field>
    </v-row>
    <v-row>
      <v-text-field label="Nama" variant="outlined" v-model="dos.nama"></v-text-field>
    </v-row>
    <v-row>
      <v-btn color="blue" @click="submitDosen">SUBMIT</v-btn>
    </v-row>
  </v-container>
</template>
<script lang="ts">
import { Dosen } from '@/model/dosen'
export default {
  data() {
    return {
      dos: new Dosen('', '')
    }
  },
  methods: {
    submitDosen() {
      alert('Data Dosen ' + this.dos.nama + ' berhasil disimpan')
      this.dos = new Dosen('', '')
    }
  }
}
</script>
