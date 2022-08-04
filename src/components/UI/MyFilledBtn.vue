<template>
    <button @click="this.$emit('submit')" 
    class="bg-[#F14A16] p-[0.7rem] px-9 rounded-3xl text-white 
    hover:scale-105 shadow-[#000000] shadow-[0px_10px_20px_-10px] 
    transition-all ease-in-out active:scale-100 xl:text-3xl">
        <slot></slot>
    </button>
</template>

<script>
export default {
    
}
</script>

<style scoped>
button{
    font-family: proximaBold;
}
    
</style>