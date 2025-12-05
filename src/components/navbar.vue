<script setup>
import { ref } from 'vue';
const isMobileMenuOpen = ref(false);
const navLinks = [
    { name: 'Home', href: '#home' },
    { name: 'About Me', href: '#about' },
    { name: 'Projects', href: '#projects' },
];
</script>

<template>
    <nav class="fixed top-0 w-full z-50 bg-white/80 backdrop-blur-md border-b border-gray-100 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">

                <div class="flex-shrink-0 flex items-center">
                    <a href="#" class="text-2xl font-bold text-slate-900 tracking-tighter">
                        Rigi<span class="text-indigo-600">.Dev</span>
                    </a>
                </div>

                <div class="hidden md:flex items-center space-x-8">
                    <a v-for="item in navLinks" :key="item.name" :href="item.href" class="text-sm font-medium text-slate-600 hover:text-indigo-600 transition-colors relative group">
                        {{ item.name }}
                        <span class="absolute -bottom-1 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
                    </a>
                    <a href="https://wa.me/+6281385605396"
                        class="px-5 py-2.5 text-sm font-bold text-white bg-slate-900 rounded-lg hover:bg-indigo-600 transition-all shadow-lg hover:shadow-indigo-500/30">
                        Hire Me
                    </a>
                </div>

                <div class="md:hidden flex items-center">
                    <button @click="isMobileMenuOpen = !isMobileMenuOpen" class="text-slate-600 hover:text-slate-900 focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path v-if="!isMobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6H16M5 12H16M4 18H16" />
                            <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>

        <div v-if="isMobileMenuOpen" class="md:hidden bg-white border-t border-gray-100">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a v-for="item in navLinks" :key="item.name" :href="item.href"
                    class="block px-3 py-2 rounded-md text-base font-medium text-slate-600 hover:text-indigo-600 hover:bg-gray-50">
                    {{ item.name }}
                </a>
                <a href="mailto:rigiyuda123@gmail.com"
                    class="block w-full text-center mt-4 px-3 py-3 rounded-lg text-base font-bold text-white bg-slate-900 hover:bg-indigo-600 shadow-md transition-all">
                    Hire Me
                </a>
            </div>
        </div>
    </nav>
</template>