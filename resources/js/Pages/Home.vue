<script setup>
import TwitterLayout from '@/Layouts/TwitterLayout.vue';
import Tweet from '@/Components/Tweet.vue';
import { Head, Link } from '@inertiajs/vue3';

import RiArrowDownSLine from '~icons/ri/arrow-down-s-line';
import RiEarthFill from '~icons/ri/earth-fill';

import RiGalleryLine from '~icons/ri/gallery-line';
import RiFileGifLine from '~icons/ri/file-gif-line';
import RiListRadio from '~icons/ri/list-radio';
import RiUserSmileLine from '~icons/ri/user-smile-line';
import RiCalendarCheckLine from '~icons/ri/calendar-check-line';
import RiMapPin2Line from '~icons/ri/map-pin-2-line';

import RiMoreFill from '~icons/ri/more-fill';
</script>

<template>
    <Head title="Home/Twitter" />
    <TwitterLayout>
        <div class="flex items-start">

            <!-- Main Content -->
            <div class="flex-1 h-screen border-l border-r">
                <div class="border-b border-gray-100 backdrop-blur-md bg-white/30">
                    <h1 class="px-5 py-4 text-xl font-bold">Home</h1>

                    <div class="flex items-center justify-between">
                        <Link class="text-center w-full hover:bg-gray-200 py-3.5 font-semibold relative after:absolute after:bg-blue-400 after:w-14 after:h-[4px] after:rounded-full after:bottom-0 after:left-1/2 after:-translate-x-1/2">
                            For you
                        </Link>
                        <Link class="text-center w-full hover:bg-gray-200 py-3.5 font-semibold text-gray-500 relative">
                            Following
                        </Link>
                    </div>
                </div>

                <div class="h-screen overflow-y-auto">
                    <div class="flex items-start px-5 py-3 space-x-3 border-b border-gray-100">
                        <img class="w-10 h-10 rounded-full" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQKVy7fXC26IPrrGOXVepyQiQvHEkyEHGWyjA&usqp=CAU" alt="">
                        
                        <div class="w-full">
                            <div class="w-full pb-3 border-b border-gray-100">
                                <button class="flex items-center px-3 space-x-1 font-semibold text-blue-500 border rounded-full">
                                    <span>Everyone</span>
                                    <RiArrowDownSLine />
                                </button>

                                <input type="text" placeholder="What is happening?" class="w-full pl-0 mt-3 mb-2 text-xl border-none focus:ring-0 focus:outline-none">
                                
                                <button class="flex items-center px-2 space-x-1 font-semibold text-blue-500 rounded-full hover:bg-blue-50">
                                    <RiEarthFill />
                                    <span>Everyone can reply</span>    
                                </button>
                            </div>

                            <div class="flex items-center justify-between py-2">
                                <div class="flex space-x-1 text-blue-500">
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiGalleryLine /></button>
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiFileGifLine /></button>
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiListRadio /></button>
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiUserSmileLine /></button>
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiCalendarCheckLine /></button>
                                    <button class="p-2 hover:bg-blue-50 hover:rounded-full"><RiMapPin2Line /></button>
                                </div>
                                <button class="px-4 py-1.5 font-semibold text-white bg-blue-300 rounded-full">Tweet</button>
                            </div>
                        </div>
                    </div>
                    
                    <button class="w-full py-3 font-normal text-center text-blue-400 duration-200 border-b border-gray-100 hover:bg-gray-50">Show 375 Tweets</button>
                    
                    <!-- Tweets -->
                    <div>
                        <Tweet />
                        <Tweet />
                        <Tweet />
                        <Tweet />
                        <Tweet />
                        <Tweet />
                        <Tweet />
                    </div>
                </div>
            </div>

            <!-- Trending -->
            <aside class="pl-8 space-y-3 w-96">
                <!-- Search -->
                <div class="p-3 text-sm bg-gray-100 rounded-full">Search Twitter</div>

                <div class="h-screen overflow-y-auto">
                    <!-- Verification banner -->
                    <div class="p-3 pb-5 rounded-lg bg-slate-50">
                        <h1 class="text-xl font-extrabold">Get Verified</h1>
                        <h2 class="mt-1 mb-3 font-bold">Subscribe to unlock new features.</h2>

                        <Link class="w-full px-5 py-2 font-bold text-white bg-black rounded-full">Get Verified</Link>
                    </div>

                    <!-- Trending hashtags -->
                    <div class="rounded-lg bg-slate-50">
                        <h1 class="p-3 text-xl font-extrabold">Trends for you</h1>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>
                        
                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>

                        <Link>
                            <div class="flex items-start justify-between p-3 hover:bg-gray-100">
                                <div class="">
                                    <p class="text-sm font-thin text-gray-400">Trending in the Philippines</p>
                                    <h2 class="text-lg font-black">Alex</h2>
                                    <p class="text-sm font-thin text-gray-400">203K Tweets</p>
                                </div>

                                <button class="p-2 hover:bg-blue-50 hover:text-blue-500 hover:rounded-full"><RiMoreFill /></button>
                            </div>
                        </Link>
                    </div>
                </div>
            </aside>
        </div>
    </TwitterLayout>
</template>
