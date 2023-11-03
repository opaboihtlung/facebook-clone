<script setup>
import { Head, usePage, Link } from '@inertiajs/vue3';
import MainNavLayout from '@/Layouts/MainNavLayout.vue';
import CreatePostBox from '@/Components/CreatePostBox.vue'
import Post from '@/Components/Post';


import Magnify from 'vue-material-design-icons/Magnify.vue'
import TelevisionPlay from 'vue-material-design-icons/TelevisionPlay.vue'
import StorefrontOutline from 'vue-material-design-icons/StorefrontOutline.vue'
import AccountGroup from 'vue-material-design-icons/AccountGroup.vue'
import AccountMultiple from 'vue-material-design-icons/AccountMultiple.vue'
import Flag from 'vue-material-design-icons/Flag.vue'
import ClockTimeTwoOutline from 'vue-material-design-icons/ClockTimeTwoOutline.vue'
import Restore from 'vue-material-design-icons/Restore.vue'
import VideoImage from 'vue-material-design-icons/VideoImage.vue'
import DotsHorizontal from 'vue-material-design-icons/DotsHorizontal.vue'

const user = usePage().props.auth.user
</script>

<template>
    <Head title="Posts" />

    <MainNavLayout>
        <div class="fixed w-full h-[100%] bg-[#F1F2F5]">
            <div class="grid grid-rows-3 grid-flow-col w-full max-w-[1600px] mt-[56px] h-[calc(100%-56px)] mx-auto px-4">
                <div id="LeftSection" class="xl:w-[345px] lg:block hidden">
                    <div class="pt-4 max-w-[320px] pr-4">
                        <Link href="/" class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] p-2 rounded-md">
                            <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/87/300/320" > 
                            <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Mr. Opa
                            </div>
                        </Link>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <AccountMultiple :size="40" fillColor="#5BD7C6"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Friends
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <Flag :size="40" fillColor="#F2682C"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Pages
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <ClockTimeTwoOutline :size="40" fillColor="#21AAFA"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Most Recent
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <AccountGroup :size="40" fillColor="#20A9FD"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Groups
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <StorefrontOutline :size="40" fillColor="#48C0D8"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Marketplace
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <TelevisionPlay :size="40" fillColor="#9739CF"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Watch
                                </div>
                            </button>
                            <button class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] px-2 py-1.5 rounded-md">
                                <Restore :size="40" fillColor="#32B4D0"/>
                                <div class="text-[15px] text-gray-800 font-extrabold pl-3">
                              Memories
                                </div>
                            </button>
                    </div>
                </div>
                    <div id="PostsSection" class="row-span-6 max-w-[600px] lg:mx-0 mx-auto overflow-auto">
                       <CreatePostBox 
                            image="https://picsum.photos/id/140/300/320"
                            placeholder="What's on your mind Mr Opa"
                       />
                       <Post/>
                    </div>
                    <div id="RightSection" class="pl-4 md:block hidden">
                        <div class="max-w-[340px] min-w-[250px] mx-auto pt-4">
                            <div class="flex items-center justify-between border-b border-b-gray-300">
                                <div class="font-semibold">Contacts</div>
                                <div class="flex items-center">
                                    <div class="p-2 hover:bg-gray-300 rounded-full cursor-pointer">
                                        <VideoImage :size="23" fillColor="#050505"/> 
                                    </div>
                                    <div class="p-2 hover:bg-gray-300 rounded-full cursor-pointer">
                                        <Magnify :size="23" fillColor="#050505"/> 
                                    </div>
                                    <div class="p-2 hover:bg-gray-300 rounded-full cursor-pointer">
                                        <DotsHorizontal :size="23" fillColor="#050505"/> 
                                    </div>
                                </div>
                            </div>
                                <div class="h-[calc(100vh-115px)] overflow-auto pt-2">
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/140/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Cristiano Ronaldo</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/141/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Lionel Messi</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/142/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Neymer Junior</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/143/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Karim Benzema</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/144/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Zlatan Ibrahimović</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/145/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Robert Lewandowski</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/146/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Kylian Mbappé</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/147/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Luis Suarez</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/149/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Sergio Ramos</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/151/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Franck Ribery</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/152/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Manuel Neuer</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/153/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Gareth Bale</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/154/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Angel Di Maria</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/155/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Eden Hazard</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/156/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">James Rodriguez</div>
                                    </div>
                                    <div class="flex items-center justify-start w-full cursor-pointer hover:bg-[#E5E6E9] py-2 rounded-md">
                                        <img class="rounded-full ml-1 min-w-[38px] max-h-[38px]" src="https://picsum.photos/id/157/300/320" > 
                                        <div class="text-[15px] text-gray-800 font-extrabold pl-3">Christian Eriksen</div>
                                    </div>
                                </div>
                        </div>
                    </div>
            </div>
        </div>
    </MainNavLayout>

</template>
