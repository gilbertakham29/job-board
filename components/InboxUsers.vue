<template>
    <div class="flex items-center p-2 bg-white rounded-md mb-2">
                    <img class="w-12 h-12 rounded-full mr-1" :src=prop1 alt="Rounded avatar"/>
                    <div class="w-full">
                        <div class="flex justify-between items-center">
                            <h4 class="font-bold">{{ prop2 }}</h4>
                            <p class="text-gray-600 text">{{ prop3 }} days ago</p>
                        </div>
                        <p class="text-gray-600">Job: {{ prop4 }}</p>
                        <p class="text-gray-600">
                            {{ prop5 }}
                        </p>
                    </div>
                </div>
</template>

<script>
    export default {
        props:{
            prop1:String,
            prop2:String,
            prop3:Number,
            prop4:String,
            prop5:String
        },
        data(){
            return{

            }
        }
    }
</script>

<style lang="scss" scoped>

</style>