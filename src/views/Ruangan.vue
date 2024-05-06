<template>
  <div>
    <h1>Entry Ruangan</h1>
    <v-form @submit="submitForm">
      <v-text-field v-model="kode" label="Kode" required></v-text-field>
      <v-text-field v-model="nama" label="Nama Ruangan" required></v-text-field>
      <v-btn type="submit">Submit</v-btn>
    </v-form>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
export default defineComponent({
  name: 'Ruangan',
  setup() {
    const kode = ref('')
    const nama = ref('')
    const submitForm = () => {
      if (kode.value && nama.value) {
        alert(`Data Ruangan ${nama.value} berhasil disimpan`)
      } else {
        alert('Field belum terisi')
      }
    }
    return { kode, nama, submitForm }
  }
})
</script>
