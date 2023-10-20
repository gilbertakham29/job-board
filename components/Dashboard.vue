<template>
    <div class="sm:ml-64 bg-gray-100 md:h-screen md:overflow-hidden">
        <div class="mt-2">
            <section class="md:flex items-center justify-between md:mx-5 mx-2">
                <div>
                    <div class="flex items-center">
                        <h2 class="text-xl  font-bold">
                            Senior Product Designer
                        </h2>
                    </div>
                    <p class="text-sm text-gray-600">Purwokerto . Full Time</p>
                </div>
                <div class="mt-2 md:mt-0">
                    <button type="button" class="focus:outline-none text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-600 dark:hover:bg-green-700 dark:focus:ring-green-800">Share & Promote</button>
                    <button type="button" class="focus:outline-none text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-green-600 dark:hover:bg-green-700 dark:focus:ring-green-800">Published</button>
                </div>
            </section>
            <div class="flex flex-wrap justify-between md:w-6/12 md:mx-5 mx-2 mt-5 mb-1">
                <p class="font-bold">Candidate</p>
                <p class="font-bold text-gray-500">Job Details</p>
                <p class="font-bold text-gray-500">Time Line</p>
                <p class="font-bold text-gray-500">Hiring Team</p>
                <p class="font-bold text-gray-500">Settings</p>
            </div>
            <hr>
            <section class="md:mx-5 mx-2 mt-5 md:flex justify-between items-center">
                <div class="flex items-center">
                    <p class="font-bold">Total Candidates: </p>
                    <button class="bg-green-700 rounded-sm px-1 ml-2 text-white font-bold">22</button>
                </div>
                <div class="flex bg-gray-400 w-fit p-1 rounded-lg cursor-pointer mt-2 md:mt-0">
                    <p class="px-3 py-1 font-bold bg-white rounded-md">
                        Pipeline view
                    </p>
                    <p class="px-3 py-1 font-bold text-gray-800">Table view</p>
                </div>
            </section>
            <section class="grid grid-cols-12 gap-2 mt-5">
                <div  class="md:mx-5 mx-2 col-span-12 md:col-span-3" >
                    <div>
                        <section class="flex justify-between items-center mb-5 p-3 border-t-4 rounded-md border-green-500 bg-white">
                            <h2 class="font-bold">New Applied</h2>
                            <p class="font-bold">10</p>
                        </section>
                        <div v-for="(item,index) in userDataOne" :key="index">
                            <DasboardSection  :prop1="item.photo" :prop2="item.name" :prop3="item.days" />

                        </div>
                   
                    </div>
                </div>
                <div  class="md:mx-5 mx-2 col-span-12 md:col-span-3" >
                    <div>
                        <section class="flex justify-between items-center mb-5 p-3 border-t-4 rounded-md border-yellow-500 bg-white">
                            <h2 class="font-bold">Screening</h2>
                            <p class="font-bold">3</p>
                        </section>
                        <div v-for="(item,index) in userDataTwo" :key="index">
                            <DasboardSection  :prop1="item.photo" :prop2="item.name" :prop3="item.days" />

                        </div>
                   
                    </div>
                </div>
                <div  class="md:mx-5 mx-2 col-span-12 md:col-span-3" >
                    <div>
                        <section class="flex justify-between items-center mb-5 p-3 border-t-4 rounded-md border-orange-500 bg-white">
                            <h2 class="font-bold">Design Challenge</h2>
                            <p class="font-bold">12</p>
                        </section>
                        <div v-for="(item,index) in userDataOne" :key="index">
                            <DasboardSection  :prop1="item.photo" :prop2="item.name" :prop3="item.days" />

                        </div>
                   
                    </div>
                </div>
                <div  class="md:mx-5 mx-2 col-span-12 md:col-span-3" >
                    <div>
                        <section class="flex justify-between items-center mb-5 p-3 border-t-4 rounded-md border-violet-500 bg-white">
                            <h2 class="font-bold">Interview</h2>
                            <p class="font-bold">2</p>
                        </section>
                        <div v-for="(item,index) in userDataThree" :key="index">
                            <DasboardSection  :prop1="item.photo" :prop2="item.name" :prop3="item.days" />

                        </div>
                   
                    </div>
                </div>
            </section>
        </div>
    </div>
</template>

<script>
   export default{
    data(){
        return{
            
            userDataOne:[
            {
          photo: 'https://flowbite.com/docs/images/people/profile-picture-5.jpg',

          name: 'Esther Gongela',
          days:  1,

        },
        {
            photo:'https://flowbite.com/docs/images/people/profile-picture-1.jpg',
  
            name:'Lubrica Fannandes',

            days: 2,

        },
        {
            photo:'https://flowbite.com/docs/images/people/profile-picture-2.jpg',

            name: 'Ariyana Grozza',

            days: 2,

        },
        {
            photo: 'https://flowbite.com/docs/images/people/profile-picture-3.jpg',

            name: 'John Morchien',

            days: 3,

        }
    
],
userDataTwo:[
    {
        photo:"https://flowbite.com/docs/images/people/profile-picture-3.jpg",
        name:"Roushan Ambani",
        days:1
    },
    {
        photo:"https://flowbite.com/docs/images/people/profile-picture-4.jpg",
        name:"Rubayet Jaman",
        days:2
    },
    {
        photo:"https://flowbite.com/docs/images/people/profile-picture-1.jpg",
        name:"Ray Mistirayo",
        days:2
    }
],
userDataThree:[
{
        photo:"https://flowbite.com/docs/images/people/profile-picture-3.jpg",
        name:"Shown Micalle",
        days:1
    },
    {
        photo:"https://flowbite.com/docs/images/people/profile-picture-4.jpg",
        name:"Stone Cold",
        days:2
    },
]
        }
    }
   }
</script>

<style lang="scss" scoped>

</style>