<template>
    
<div class="sm:ml-64 bg-gray-100 md:h-screen md:overflow-hidden">
    <div>
        <div class="flex px-4 py-3">
            <h2 class="mr-5 text-blue-600 font-bold">RECRUITMENT INBOX</h2>
            <h2 class="text-gray-600 font-bold">WORK INBOX</h2>
        </div>
        <hr>
        <div class="grid grid-cols-12">
            <section class="col-span-12 md:col-span-3 md:px-4 px-2 py-4 md:border-r">
                <div class="flex items-center mb-4">
                    <form class="w-full mr-4">
                        <label for="default-search" class="mb-2 text-sm font-medium text-gray-900 sr-only dark:text-white">Search</label>
                        <div class="relative">
                            <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 text-gray-500 dark:text-gray-400">
  <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
</svg>

                            </div>
                            <input type="search" id="default-search" class="block w-full p-2.5 pl-10 text-sm text-gray-900 border border-gray-300 rounded-lg bg-gray-50 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
                        </div>
                    </form>
                    <div class="p-2 border rounded-md text-gray-500">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M12 3c2.755 0 5.455.232 8.083.678.533.09.917.556.917 1.096v1.044a2.25 2.25 0 01-.659 1.591l-5.432 5.432a2.25 2.25 0 00-.659 1.591v2.927a2.25 2.25 0 01-1.244 2.013L9.75 21v-6.568a2.25 2.25 0 00-.659-1.591L3.659 7.409A2.25 2.25 0 013 5.818V4.774c0-.54.384-1.006.917-1.096A48.32 48.32 0 0112 3z" />
</svg>

                    </div>
                </div>
                <div v-for="(item,index) in inboxData" :key="index">
                    <InboxUsers :prop1="item.photo" :prop2="item.name" :prop3="item.days" :prop4="item.job" :prop5="item.role"/>
                </div>
                
            </section>
            <section class="lg:col-span-6 col-span-12 md:col-sapn-3 pt-4 md:border-r">
                <div class="flex justify-between items-center md:px-4 px-2 pb-4">
                    <div>
                        <h5 class="text-sm font-bold">My Application for Senior Developer</h5>
                        <p>Job: Front-End Developer</p>
                    </div>
                    <div class="flex bg-gray-400 w-fit p-1 rounded-lg cursor-pointer mt-2 md:mt-0">
                        <p class="px-3 py-1 font-bold bg-white rounded-md">Chat</p>
                        <p class="px-3 py-1 font-bold text-gray-800">Email</p>
                    </div>
                </div>
                <hr>
                <div class="inline-flex items-center justify-center w-full relative">
                    <hr class="w-full h-px my-8 bg-gray-200 border-0 dark:bg-gray-700">
                    <span class="absolute px-3 font-medium text-white -translate-x-1/2 bg-black rounded-full py-1 left-1/2 text-xs">Fri,2 Jul</span>
                </div>
                <div class="md:px-4 px-2">
                    <p class="bg-white p-2 rounded-lg md:w-7/12 w-11/12">
                    Hello, Here is the file you required before. Please, Checkout this assessment, and let me know if you need something else.
                    </p> 
                </div>
                <div class="md:px-4 px-2 mt-4">
                    <div class="bg-white p-2 rounded-lg md:w-7/12 w-11/12 flex justify-between items-center">
                        <div class="flex items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mr-2">
  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 14.25v-2.625a3.375 3.375 0 00-3.375-3.375h-1.5A1.125 1.125 0 0113.5 7.125v-1.5a3.375 3.375 0 00-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 00-9-9z" />
</svg>
<div>
    <p class="font-bold">CV New.doc</p>
    <p class="text-gray-600">1.2 Mb</p>
</div>

                        </div>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M3 16.5v2.25A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75V16.5M16.5 12L12 16.5m0 0L7.5 12m4.5 4.5V3" />
</svg>

                    </div>
                </div>
<div class="inline-flex items-center justify-center w-full relative">
    <hr class="w-full h-px my-8 bg-gray-200 border-0 dark:bg-gray-700">
    <span class="absolute px-3 font-medium text-white -translate-x-1/2 bg-black rounded-full py-1 left-1/2 text-xs">Today</span>
</div>
<div class="md:px-4 px-2 flex justify-end">
    <p class="bg-green-300 p-2 rounded-lg md:w-7/12 w-11/12">
        Hello Cody, Thank you, I will check it out and let you know if we need something else. Thanks.
    </p>
</div>
<div class="md:px-4 px-2 mt-4">
    <p class="bg-white p-2 rounded-lg md:w-7/12 w-11/12">Thank you, I will wait for your feedback, Thanks.</p> 
</div>
<Message/>
            </section>
            <section class="lg:col-span-3 col-span-12 md:col-span3 py-4">
                <div class="flex justify-center">
                    <img class="w-16 h-16 rounded-full" src="https://flowbite.com/docs/images/people/profile-picture-3.jpg" alt="Rounded avatar">
                </div>
                <h3 class="text-center font-bold mt-2">Cody Fisher</h3>
                <p class="text-sm text-center text-gray-600 mb-4">View Profile</p>
                <hr>
                <div class="md:px-4 px-2 py-4">
                    <h5 class="text-xs font-bold">Applied For:</h5>
                    <h5 class="font-bold">Job: Senior UIX Designer</h5>
                    <p class="text-gray-600 text-sm">Design Team</p>
                    <div class="flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 text-yellow-400">
  <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
</svg>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 text-yellow-400">
  <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
</svg>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 text-yellow-400">
  <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
</svg>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 text-yellow-400">
  <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
</svg>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-5 h-5 text-gray-300">
  <path fill-rule="evenodd" d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z" clip-rule="evenodd" />
</svg>

                    </div>
                </div>
                <hr>
                <div class="md:px-4 px-2 py-4">
                    <p class="flex items-center mb-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mr-1">
  <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
</svg>
codyfish@gmail.com
                    </p>
                    <p class="flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 mr-1">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 01-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z" />
</svg>
+916482354685
                    </p>
                </div>
                <hr>
                <div class="md:px-4 px-2 py-4">
                    <p class="flex items-center text-blue-600 font-bold">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M12 9v6m3-3H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z" />
</svg>
Add Owner
                    </p>
                </div>
                <hr>
                <div class="md:px-4 px-2 py-4">
                    <h2 class="text-sm font-bold">Schedule:</h2>
                    <div class="mt-2 border border-l-4 p-2 border-l-green-400 rounded-md">
                        <h2 class="font-bold mb-2 text-gray-700">Alignment for onboarding welcoming new member on Product Teams</h2>
                        <span class="bg-blue-100 text-blue-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded dark:bg-gray-700 dark:text-blue-400 border border-blue-400">Waiting Approval</span>
                        <p class="mt-2 text-sm">9 Mar, 2021 7:00-7:45pm</p>

                        <p class="text-xs font-bold mt-4">View Summary</p>
                    </div>
                </div>
            </section>
        </div>
    </div>
</div>
</template>

<script>
    export default {
        data(){
            return{
                inboxData:[
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-1.jpg",
                name:"Brooklyn Simmons",
                days:1,
                job:"Senior UIX Designer",
                role:"Design Team"
            },
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-2.jpg",
                name:"Ronaldo Karvia",
                days:1,
                job:"UI/UX Designer",
                role:"Design Team"
            },
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-3.jpg",
                name:"Coddy Fisher",
                days:2,
                job:"Front-End Developer",
                role:"Developer Team"
            },
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-4.jpg",
                name:"Airlen McKoi",
                days:3,
                job:"Web Designer",
                role:"Design Team"
            },
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-5.jpg",
                name:"Darlane Robert",
                days:3,
                job:"Web Designer",
                role:"Design Team"
            },
            {
                photo:"https://flowbite.com/docs/images/people/profile-picture-2.jpg",
                name:"Robarto Carlose",
                days:3,
                job:"Web Developer",
                role:"Developer Team"
            },
        ]
            }
        }
       
    }
</script>

<style lang="scss" scoped>

</style>