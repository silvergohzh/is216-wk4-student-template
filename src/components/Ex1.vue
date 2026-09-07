<script setup>
    import { ref } from 'vue'

    // Add code here
    // challenge: use array  
    const message = ref("Choose your favorite fruit:")
    const fruits = ref(['apple', 'orange', 'peach'])
    // const fruit1 = ref('apple')
    // const fruit2 = ref('orange')
    // const fruit3 = ref('peach')


   
    
</script>

<template>

<!-- {{ message }}  -->
<!-- 
    <label for=""> <input type="radio" name="fruit"> {{ fruits[0] }} </label> 
    <label for=""> <input type="radio" name="fruit"> {{  fruits[1] }} </label> 
    <label for=""><input type="radio" name="fruit"> {{  fruits[2] }} </label>  -->

    <br>
    {{message}}
    <label v-for="(fruit, index) in fruits" :key="index">
        <input type="radio" name="fruit" :value="fruit"> {{ fruit }}
    </label>
    
</template>

<style scoped>
</style>
