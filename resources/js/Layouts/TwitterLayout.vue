<script setup>
import MenuItems from '@/Components/MenuItems.vue';
import { Link } from '@inertiajs/vue3';
import { ref } from 'vue';
</script>

<template>
    <div class="max-w-[1223px] mx-auto">
        <div class="flex items-start">

            <MenuItems />

            <!-- Main -->
            <main class="flex-1">
                <slot />
            </main>
        </div>
    </div>
</template>
