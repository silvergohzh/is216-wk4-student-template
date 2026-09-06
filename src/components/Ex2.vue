<script setup>
    import { ref } from 'vue'

    // Add code here

    const me = ref('/assets/me.png')
    const width = ref(200)
   

    const v2 = ref({
        src: '/assets/me.png',
        width: 200,
        
    })

</script>

<template>

    <!-- Add code here -->
     
    <img v-bind:src="me" v-bind:width="width" >

    <img v-bind="v2">
     

</template>
