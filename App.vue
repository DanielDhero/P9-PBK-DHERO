<script>
  import mobil from './components/mobil.vue'

  export default { 
    components : {
      mobil
    },
    data() {
      return {
        mobilyangdipilih: ''
        }
      },
      methods: {
        tampildata(whatever){
          this.mobilyangdipilih = whatever
        }
      }
    }
</script>

<template>
  <mobil @tampil="tampildata" namamobil="Kijang">Ini merupakan konten dari komponen induk</mobil>> 
  <br>
  <mobil @tampil="tampildata" namamobil="Avanza">Ini merupakan konten dari komponen induk</mobil>>
  <br>
  <mobil @tampil="tampildata" namamobil="Pajero">Ini merupakan konten dari komponen induk</mobil>>

  <p>Mobil yang anda pilih: {{ mobilyangdipilih }} </p>
</template>

<style>
</style>
