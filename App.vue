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
  <mobil @tampil="tampildata" namamobil="Kijang"/> 
  <br>
  <mobil @tampil="tampildata" namamobil="Avanza"/>
  <br>
  <mobil @tampil="tampildata" namamobil="Pajero"/>

  <p>Mobil yang anda pilih: {{ mobilyangdipilih }} </p>
</template>

<style>
</style>
