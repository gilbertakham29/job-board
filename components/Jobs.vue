<template>
    <div class="sm:ml-64 bg-gray-100 md:h-screen md:overflow-hidden">
        <div>
            <div class="flex flex-col gap-2">
                <div aria-label="Default tabs" role="tablist" class="flex text-center flex-wrap border-b border-gray-200 dark:border-gray-700">
                    <button type="button" aria-controls=":r0:-tabpanel-0" aria-selected="true" class="flex items-center justify-center p-4 text-sm font-medium first:ml-0 disabled:cursor-not-allowed disabled:text-gray-400 disabled:dark:text-gray-500 base active bg-gray-100 text-blue-600 dark:bg-gray-800 dark:text-blue-500" role="tab" tabindex="0">Active Jobs</button>
                    <button type="button" aria-controls=":r0:-tabpanel-1" aria-selected="false" class="flex items-center justify-center p-4 text-sm font-medium first:ml-0 disabled:cursor-not-allowed disabled:text-gray-400 disabled:dark:text-gray-500 base active text-gray-500 hover:bg-gray-50 hover:text-gray-600 dark:text-gray-400 dark:hover:bg-gray-800  dark:hover:text-gray-300" id=":rg:-tab-1" role="tab" tabindex="-1">Inactive Jobs</button>
                </div>
                <div>
                    <div role="tabpanel" tabindex="0">
                        <div>
                            <div class="md:flex items-center mb-5">
                                <h3 class="text-2xl font-bold md:mr-10 mb-1">7 Active Jobs</h3>
                                <p class="text-gray-600 flex items-center mr-10">
                                    Short by:
                                    <span class="font-bold text-sm text-black flex items-center ml-2">
                                    Creation Date
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 15L12 18.75 15.75 15m-7.5-6L12 5.25 15.75 9" />
</svg>

                                </span>
                                </p>

                                <p class="text-gray-600 flex items-center mr-10">
                                    Status:
                                    <span class="font-bold text-sm text-black flex items-center ml-2">
                                    All Status
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 15L12 18.75 15.75 15m-7.5-6L12 5.25 15.75 9" />
</svg>

                                </span>
                                </p>
                               
                            </div>
                            <section class="grid grid-cols-12 gap-5">
                                <div v-for="(item,index) in jobsData" :key="index" class="border-t-4 border-orange-500 p-2 col-span-12 md:col-span-3 bg-white rounded-md">

                                    <JobSection :prop1="item.job" :prop2="item.role" :prop3="item.total" :prop4="item.new"/>
                                </div>
                             
                            </section>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                jobsData:[
                    {
                        job:"Design",
                        role:"Senior Product Designer",
                        total:36,
                        new:5,
                    },
                    {
                        job:"Design",
                        role:"UI/UX Designer",
                        total:23,
                        new:2,
                    },
                    {
                        job:"Developer",
                        role:"Senior Developer",
                        total:42,
                        new:2,
                    },
                    {
                        job:"Design",
                        role:"Head of UX",
                        total:16,
                        new:4,
                    },
                    {
                        job:"Marketing",
                        role:"Copy Writer",
                        total:27,
                        new:9,
                    },
                    {
                        job:"Design",
                        role:"Senior Product Designer",
                        total:36,
                        new:5,
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>