<template>
                                    <h4 class="font-bold text-2xl text-gray-600">{{ prop1 }}</h4>
                                    <h4 class="font-bold">{{ prop2 }}</h4>
                                    <h6 class="text-sm text-gray-600 mt-3">Candidates:</h6>
                                    <div class="mt-1 grid grid-cols-2 items-center border-2 p-2 bg-slate-300 rounded-md">
                                        <div class="px-1 border-l-4 border-green-500">
                                            <p class="text-sm font-bold text-gray-600">TOTAL</p>
                                            <h3 class="text-lg font-bold">{{ prop3 }}</h3>
                                        </div>
                                        <div class="px-1 border-l-4 border-green-500">
                                            <p class="text-sm font-bold text-gray-600">NEW</p>
                                            <h3 class="text-lg font-bold">{{ prop4 }}</h3>
                                        </div>
                                    </div>
                                    <p class="text-lg font-bold text-gray-700 my-1 text-center">
                                        Purwokerto . Freelancer
                                    </p>
                                    <hr>
                                    <div class="flex justify-between mt-2">
                                        <p class="flex items-center text-gray-700">
                                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M9 12h3.75M9 15h3.75M9 18h3.75m3 .75H18a2.25 2.25 0 002.25-2.25V6.108c0-1.135-.845-2.098-1.976-2.192a48.424 48.424 0 00-1.123-.08m-5.801 0c-.065.21-.1.433-.1.664 0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75 2.25 2.25 0 00-.1-.664m-5.8 0A2.251 2.251 0 0113.5 2.25H15c1.012 0 1.867.668 2.15 1.586m-5.8 0c-.376.023-.75.05-1.124.08C9.095 4.01 8.25 4.973 8.25 6.108V8.25m0 0H4.875c-.621 0-1.125.504-1.125 1.125v11.25c0 .621.504 1.125 1.125 1.125h9.75c.621 0 1.125-.504 1.125-1.125V9.375c0-.621-.504-1.125-1.125-1.125H8.25zM6.75 12h.008v.008H6.75V12zm0 3h.008v.008H6.75V15zm0 3h.008v.008H6.75V18z" />
</svg>
Draft
                                        </p>
                                        <p class="text-gray-700">See Details</p>
                                    </div>
                             
                                
</template>

<script>
    export default {
        props:{
            prop1:String,
            prop2:String,
            prop3:Number,
            prop4:Number,
        },
        data(){
            return {

            }
        }
    }
</script>

<style lang="scss" scoped>

</style>