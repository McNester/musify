<template >
    <div class="bg-[#370665] w-full pl-10 pt-5 pb-10 flex items-start flex-col">
        <h1 class="heading">Contact us</h1>
        <h1>1800-102-0525</h1>
        <h1>Mon-Sun- 10AM-7PM</h1>

        <h1 class="heading mt-5">Manufactured by: </h1>
        <h1 class="w-[40%]">Harman International Industries, Inc. 8500, Balboa Blvd, Northridge, CA 91329,USA</h1>

        <h1 class="heading mt-10">Share on Social Media</h1>
        <div class="flex justify-center items-center gap-5 pt-3">
            <img class="media" src="/imgSrc/google.png">
            <img class="media" src="/imgSrc/insta.png" >
            <img class="media" src="/imgSrc/twitter.png">
        </div>

        <h1 class="heading mt-5 mb-3">Subscribe to our Newsletter</h1>
        <div class="flex flex-col justify-center items-start gap-5">
            <MyInput v-model:text="email" ></MyInput>
            <MyFilledBtn @submit="clearInput" id="subscribe">Subscribe</MyFilledBtn>
        </div>

        <img src="/imgSrc/footerLogo.png" class=" self-center -ml-10">
        
        <h1 class="heading self-center -ml-10">© 2022.Musify.All Rights Reserved</h1>
        
    </div>
</template>

<script>
import MyInput from './MyInput.vue';
import MyFilledBtn from './MyFilledBtn.vue';
export default {
    components: { MyInput, MyFilledBtn },
    data() {
        return {
            email: ""
        }
    },
    methods: {
        clearInput() {
            this.email = "";
        }
    },
}
</script>

<style scoped>
.media{
    @apply scale-75 hover:scale-[0.8] active:scale-75 cursor-pointer
}
h1{
    color: white;
    font-family: proximaLight;
}
.heading{
    font-family: proximaBold;
}
#subscribe{
    @apply p-[0.3rem] px-6 rounded-xl shadow-2xl ml-1
}
</style>