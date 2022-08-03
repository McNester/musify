<template >
    <div>
        <input 
        :value="text"
        @input="updateInput"

        type="text" 
        class=" border-2 border-[#F14A16] p-1 pl-3 pr-5 bg-transparent 
        rounded-[0.9rem] outline-none" 
        placeholder="Enter your mail id">
    </div>
</template>
<script>
export default {
    props:{
        text:String
    },
    methods: {
        updateInput(event){
            this.$emit('update:text',event.target.value)
        }
    }
    
}
</script>
<style scoped>
input{
    font-family: proximaLight;
    color: white;
}
</style>