<script setup>
    import { ref } from 'vue'

    // Add code here

    const me = ref('/assets/me.png')
    const width = ref('200')
    const height = ref('200')
   

    // multiple attribute binding
    const obj = ref({
        width: '200',
        height: '200',
        src: '../../public/assets/me.png'
        
    })

</script>

<template>

    <!-- Add code here -->
     
    <img v-bind:src="me" v-bind:width="width" v-bind:height="height" >

    <img v-bind="obj">
     

</template>
