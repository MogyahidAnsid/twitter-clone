<template>
    <div>
        <Link href="#">
            <div class="flex items-start w-full px-5 py-3 space-x-3 border-b border-gray-100 hover:bg-gray-100">
                <img class="w-10 h-10 rounded-full" src="https://avatars.githubusercontent.com/u/66927676?v=4" alt="">

                <div class="flex-1">
                    <div class="flex items-center space-x-1">
                        <h1 class="font-extrabold">John Doe</h1>
                        <h3 class="text-gray-500">@john_doe <span> • 11m</span></h3>
                    </div>

                    <div class="mt-1">
                        <p>
                            🔥 Did you know you can preview an e-mail with Laravel?

                            You just need to return an instance of the Mail class and the response is going to be an HTML preview of the exact e-mail.
                            
                            Exactly what I needed for a newsletter feature and it's very helpful for debugging:
                        </p>
                    </div>

                    <div class="flex items-center justify-between mt-3 text-gray-500">
                        <button class="flex items-center space-x-2 group">
                            <RiChat1Line class="p-1.5 rounded-full w-8 h-8 group-hover:bg-blue-50 group-hover:text-blue-500"/>
                            <span class="group-hover:text-blue-500">1</span>
                        </button>
                        <button class="flex items-center space-x-2 group">
                            <RiArrowUpDownLine class="p-1.5 rounded-full w-8 h-8 group-hover:bg-blue-50 group-hover:text-blue-500"/>
                        </button>
                        <button class="flex items-center space-x-2 group">
                            <RiHeart3Line class="p-1.5 rounded-full w-8 h-8 group-hover:bg-red-50 group-hover:text-red-500"/>
                            <span class="group-hover:text-red-500">1</span>
                        </button>
                        <button class="flex items-center space-x-2 group">
                            <RiBarChartFill class="p-1.5 rounded-full w-8 h-8 group-hover:bg-blue-50 group-hover:text-blue-500"/>
                            <span class="group-hover:text-blue-500">274</span>
                        </button>
                        <button class="flex items-center space-x-2 group">
                            <RiUpload2Line class="p-1.5 rounded-full w-8 h-8 group-hover:bg-blue-50 group-hover:text-blue-500"/>
                        </button>
                    </div>
                </div>
                
                <button class="text-gray-500">
                    <RiMoreFill class="p-1.5 rounded-full w-8 h-8 hover:bg-blue-50 hover:text-blue-500"/>
                </button>
            </div>
        </Link>
    </div>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';

import RiMoreFill from '~icons/ri/more-fill';
import RiChat1Line from '~icons/ri/chat-1-line';
import RiArrowUpDownLine from '~icons/ri/arrow-up-down-line';
import RiHeart3Line from '~icons/ri/heart-3-line';
import RiBarChartFill from '~icons/ri/bar-chart-fill';
import RiUpload2Line from '~icons/ri/upload-2-line';
</script>