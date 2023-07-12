<template>
    <div class="flex flex-col justify-between h-screen pr-3 mt-1 w-72">
        <!-- Menu Item -->
        <div class="flex flex-col items-start justify-start pr-10 text-xl">
            <Link href="/home" class="inline-block p-3 text-3xl text-blue-500 rounded-full hover:bg-gray-200"><RiTwitterFill /></Link>
            <Link 
                v-for="item in navItems" :key="item.name" 
                class="inline-flex items-center px-4 py-3 space-x-5 duration-300 rounded-full hover:bg-gray-200"
                :class="{'font-extrabold': route().current(item.href), 'text-gray-600' : !route().current(item.href)}">
                <component :is="route().current(item.href) ? item.activeIcon : item.icon" />
                <span>{{ item.name }}</span>
            </Link>

            <button class="w-full px-4 py-3 mt-1 font-semibold text-white bg-blue-500 rounded-full shadow">Tweet</button>
        </div>

        <button class="flex items-center justify-between px-4 py-3 space-x-3 duration-300 rounded-full hover:bg-gray-200">
            <div class="flex items-center space-x-3">
                <img class="rounded-full w-11 h-11" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQKVy7fXC26IPrrGOXVepyQiQvHEkyEHGWyjA&usqp=CAU" alt="">

                <div class="text-left">
                    <h1 class="font-extrabold">Mogyahid</h1>
                    <h3 class="text-gray-600">@mogyahid_ansid</h3>
                </div>
            </div>

            <button><RiMoreFill /></button>
        </button>
    </div>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';

import RiTwitterFill from '~icons/ri/twitter-fill';

import RiHome2Line from '~icons/ri/home-2-line';
import RiHome2Fill from '~icons/ri/home-2-fill';

import PhMagnifyingGlass from '~icons/ph/magnifying-glass';
import PhMagnifyingGlassBold from '~icons/ph/magnifying-glass-bold';

import RiNotificationLine from '~icons/ri/notification-line';
import RiNotificationFill from '~icons/ri/notification-fill';

import RiMailLine from '~icons/ri/mail-line';
import RiMailOpenFill from '~icons/ri/mail-open-fill';

import RiFileList2Line from '~icons/ri/file-list-2-line';
import RiFileList2Fill from '~icons/ri/file-list-2-fill';

import RiBookmarkLine from '~icons/ri/bookmark-line';
import RiBookmarkFill from '~icons/ri/bookmark-fill';

import RiShieldCheckLine from '~icons/ri/shield-check-line';
import RiShieldCheckFill from '~icons/ri/shield-check-fill';

import RiUserLine from '~icons/ri/user-line';
import RiUserFill from '~icons/ri/user-fill';

import RiMoreFill from '~icons/ri/more-fill';

const navItems = [
    {
        name: 'Home',
        href: 'home',
        activeIcon: RiHome2Fill,
        icon: RiHome2Line
    },
    {
        name: 'Explore',
        href: '/',
        activeIcon: PhMagnifyingGlassBold,
        icon: PhMagnifyingGlassBold
    },
    {
        name: 'Notifications',
        href: '/',
        activeIcon: RiNotificationFill,
        icon: RiNotificationLine
    },
    {
        name: 'Messages',
        href: '/',
        activeIcon: RiMailOpenFill,
        icon: RiMailLine
    },
    {
        name: 'Lists',
        href: '/',
        activeIcon: RiFileList2Fill,
        icon: RiFileList2Line
    },
    {
        name: 'Bookmarks',
        href: '/',
        activeIcon: RiBookmarkFill,
        icon: RiBookmarkLine
    },
    {
        name: 'Verified',
        href: '/',
        activeIcon: RiShieldCheckFill,
        icon: RiShieldCheckLine
    },
    {
        name: 'Profile',
        href: '/',
        activeIcon: RiUserFill,
        icon: RiUserLine
    },
    {
        name: 'More',
        href: '/',
        activeIcon: RiMoreFill,
        icon: RiMoreFill
    },
];
</script>