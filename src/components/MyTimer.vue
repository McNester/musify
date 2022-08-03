<template >
    <div class="flex justify-center items-center">
        <div class="flex justify-center items-center flex-col">
            <div id="hours" class="timeUnit">
                {{getHours}}
            </div>
            <h1>Hour</h1>
        </div>

        <div class="flex justify-center items-center flex-col">
            <div id="minutes" class="timeUnit">
                {{getMinutes}}
            </div>
            <h1>Min</h1>
        </div>

        <div class="flex justify-center items-center flex-col">
            <div id="seconds" class="timeUnit">
                {{getSeconds}}
            </div>
            <h1 >Sec</h1>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            offerTimeMillis: 3600000
        }
    },
    computed:{
        getHours(){
            var hours = Math.floor((this.offerTimeMillis / 1000 / 3600 ) % 24)
            return this.makeTwoDigitStringTimeUnit(hours)
            
        },
        getMinutes(){
            var minutes = Math.floor((this.offerTimeMillis / 1000 / 60) % 60);
            return this.makeTwoDigitStringTimeUnit(minutes)
            
        },
        getSeconds(){
            var seconds = Math.floor((this.offerTimeMillis / 1000) % 60);
            return this.makeTwoDigitStringTimeUnit(seconds)
            
        },
        
    },
    methods: {
        makeTwoDigitStringTimeUnit(timeUnit){
            if(timeUnit < 10){
                return '0'+timeUnit
            }
            return ''+timeUnit
        },
        sendOfferEnd(){
            this.$emit('offerEnd')
        },
        runTimer(){
            let int = setInterval(()=>{
                if(this.offerTimeMillis <= 0){
                    clearInterval(int)
                    this.sendOfferEnd()
                    return;
                }
                this.offerTimeMillis -= 1000
            }, 1000);
        }
    },
    mounted() {
        this.runTimer()
    },
}
</script>

<style scoped>
.timeUnit{
    font-family: proximaBold;
    @apply w-[5rem] h-[6rem] bg-[#370665] mx-5 rounded-[2rem] 
    flex justify-center items-center text-white text-5xl
}
h1{
    font-family: proximaLight;
}
</style>