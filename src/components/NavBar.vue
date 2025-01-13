<template>
    <!-- nav container -->
    <nav class="relative mx-auto bg-cyan-700">
        <!-- items container -->
        <div class="flex px-8 md:px-8 p-4 items-center justify-between">
            <!-- logo -->
            <div class="text-2xl capitalize text-white font-medium">
                <a href="#">beauty<span class="text-cyan-300">Bliss</span></a>
            </div>

            <!-- nav items -->
            <div :class="{ 'md:flex': !isMenuOpen, 'hidden': isMenuOpen }"
                class="hidden items-center justify-center space-x-6">
                <div class="group">
                    <a href="#" class="capitalize text-sm text-white">home</a>
                    <div class="hidden border-b border-cyan-300 mx-2 group-hover:block"></div>
                </div>
                <div class="group">
                    <a href="#" class="capitalize text-sm text-white">about</a>
                    <div class="hidden border-b border-cyan-300 mx-2 group-hover:block"></div>
                </div>
                <div class="group">
                    <a href="#products" class="capitalize text-sm text-white">products</a>
                    <div class="hidden border-b border-cyan-300 mx-2 group-hover:block"></div>
                </div>
                <div class="group">
                    <a href="#blog" class="capitalize text-sm text-white">blogs</a>
                    <div class="hidden border-b border-cyan-300 mx-2 group-hover:block"></div>
                </div>
                <div class="group">
                    <a href="#" class="capitalize text-sm text-white">contact us</a>
                    <div class="hidden border-b border-cyan-300 mx-2 group-hover:block"></div>
                </div>
            </div>

            <!-- login & signup -->
            <div :class="{ 'md:flex': !isMenuOpen, 'hidden': isMenuOpen }"
                class="hidden items-center justify-center space-x-6">
                <a href="#" class="relative group flex items-center justify-between">
                    <svg class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24"
                        height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                    </svg>
                    <div
                        class="absolute -top-3 -right-3 text-cyan-700 h-5 w-5 bg-white flex items-center justify-center rounded-full">
                        2
                    </div>
                </a>
                <a href="#" class="text-white">
                    <svg class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24"
                        height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-width="2"
                            d="M7 17v1a1 1 0 0 0 1 1h8a1 1 0 0 0 1-1v-1a3 3 0 0 0-3-3h-4a3 3 0 0 0-3 3Zm8-9a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                    </svg>
                </a>

                <a href="#" class="bg-cyan-300 px-6 py-2 rounded-full hover:opacity-80 cursor-pointer">
                    Sign Up
                </a>
            </div>

            <!-- hamburger, cart, login -->
            <div :class="{ 'md:hidden': !isMenuOpen, 'block': openNav }"
                class="flex items-center justify-center space-x-4">
                <a href="#" class="relative group flex items-center justify-between">
                    <svg class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24"
                        height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                    </svg>
                    <div
                        class="absolute -top-3 -right-3 text-cyan-700 h-5 w-5 bg-white flex items-center justify-center rounded-full">
                        2
                    </div>
                </a>
                <a href="#" class="text-white">
                    <svg class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24"
                        height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-width="2"
                            d="M7 17v1a1 1 0 0 0 1 1h8a1 1 0 0 0 1-1v-1a3 3 0 0 0-3-3h-4a3 3 0 0 0-3 3Zm8-9a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                    </svg>
                </a>
                <button type="button" class="cursor-pointer" @click="!isMenuOpen && toggleNav()">
                    <svg v-if="openNav" class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                        width="24" height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M6 18 17.94 6M18 18 6.06 6" />
                    </svg>
                    <svg v-else class="w-7 h-7 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                        width="24" height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-width="2"
                            d="M5 7h14M5 12h14M5 17h14" />
                    </svg>
                </button>
            </div>
        </div>

        <!-- mobile nav -->
        <div v-if="openNav" :class="{ 'block': isMenuOpen, 'md:hidden': !isMenuOpen }"
            class="block absolute z-40 top-18 left-4 right-4 p-6 py-10 rounded-lg bg-cyan-700">
            <div class="flex flex-col items-center justify-center space-y-4">
                <a href="#" class="w-full capitalize text-white text-center hover:text-cyan-300 text-lg">home</a>
                <a href="#" class="w-full capitalize text-white text-center hover:text-cyan-300 text-lg">about</a>
                <a href="#products"
                    class="w-full capitalize text-white text-center hover:text-cyan-300 text-lg">products</a>
                <a href="#blog" class="w-full capitalize text-white text-center hover:text-cyan-300 text-lg">blogs</a>
                <a href="#" class="w-full capitalize text-white text-center hover:text-cyan-300 text-lg">contact us</a>
            </div>
            <div class="mt-8 border-t border-cyan-300"></div>

            <div class="flex flex-col items-center justify-center space-y-4 mt-4">
                <button class="bg-cyan-300 w-full px-6 py-2 rounded-full hover:opacity-80 cursor-pointer">
                    Sign Up
                </button>
            </div>
        </div>
    </nav>
    <!-- end nav container -->
</template>

<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)
const openNav = ref(false)

const toggleNav = () => {
    openNav.value = !openNav.value
}
</script>
