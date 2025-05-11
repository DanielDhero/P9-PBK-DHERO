<template>
    Ini adalah mobil {{ namamobil }} <button @click="tampildata">Pilih</button>
</template>

<script>
    export default {
        props : {
            namamobil : String 
        },
        emits : ['tampil'],
        methods : {
            tampildata() {
                this.$emit('tampil', this.namamobil);
            }
    }
}
</script>
