<script setup>
</script>

<template>
    <div class="relative overflow-hidden bg-white">

        <div class="absolute top-0 left-1/2 w-full -translate-x-1/2 h-full z-0 pointer-events-none">
            <div class="absolute top-0 right-0 w-[500px] h-[500px] bg-indigo-50 rounded-full blur-3xl opacity-60 -translatey-1/2 translate-x-1/3"></div>
            <div class="absolute bottom-0 left-0 w-[500px] h-[500px] bg-blue-50 rounded-full blur-3xl opacity-60 translate-y-1/3 -translate-x-1/3"></div>
        </div>

        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-20 pb-16 md:pt-28 md:pb-24 text-center lg:text-left">
            <div class="lg:grid lg:grid-cols-12 lg:gap-8 items-center">
                <div class="sm:text-center md:max-w-2xl md:mx-auto lg:col-span-8 lg:text-left" data-aos="fade-up" data-aos-duration="1000">
                    <div class="inline-flex items-center px-3 py-1 rounded-full border border-indigo-100 bg-indigo-50 text-indigo-600 text-sm font-semibold mb-6">
                        <span class="flex h-2 w-2 relative mr-2">
                            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-indigo-400 opacity-75"></span>
                            <span class="relative inline-flex rounded-full h-2 w-2 bg-indigo-500"></span>
                        </span>
                        Available for Hire 🚀
                    </div>

                    <h1 class="text-4xl tracking-tight font-extrabold text-slate-900 sm:text-5xl md:text-6xl lg:leading-tight">
                        Engineering Reliable
                        <span class="text-transparent bg-clip-text bg-gradient-to-r from-indigo-600 to-blue-500">Back-End logic</span>
                        & Intuitive Front-End
                    </h1>

                    <p class="mt-6 text-lg text-slate-600 leading-relaxed">
                        Mahasiswa Teknik Informatika semester 5 yang siap menerjemahkan kebutuhan bisnis menjadi fitur fungsional. Fokus pada skalabilitas sistem menggunakan <strong>Node.js</strong>, <strong>Laravel</strong>, dan <strong>Vue.js</strong>
                    </p>

                    <div class="mt-8 flex flex-col sm:flex-row gap-4 sm:justify-center lg:justify-start">
                        <a href="#projects" class="px-8 py-4 bg-slate-900 text-white font-bold rounded-xl hover:bg-slate-800 translation-all shadow-lg hover:shadow-slate-500/20 fex items-center justify-center gap-2">
                            View Projects
                            <svg xmlns="https://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="curentColor">
                                <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 016 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd" />
                            </svg>
                        </a>
                        <a href="https://github.com/RigiYS" target="_blank" class="px-8 py-4 bg-white text-slate-700 border border-slate-200 font-bold rounded-xl hover:bg-slate-50 transition-all flex items-ceter justify-center gap-2">
                            <svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                                <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.477 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .26.18.57.688.475A10.005 10.005 0 0122 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" />
                            </svg>
                            Github Profile
                        </a>
                    </div>
                </div>

                <div class="mt-12 relative sm:max-w-lg sm:mx-auto lg:mt-0 lg:max-w-none lg:mx-0 lg:col-span-4 lg:flex lg:items-center" data-aos="fade-left" data-aos-delay="300">
                    <div class="relative mx-auto w-full rounded-lg shadow-lg lg:max-w-md">
                        <div class="relative block w-full bg-white rounded-lg overflow-hidden border border-slate-200 p-6">
                            <div class="flex items-center space-x-4 mb-4">
                                <div class="h-3 w-3 bg-red-500 rounded-full"></div>
                                <div class="h-3 w-3 bg-yellow-500 rounded-full"></div>
                                <div class="h-3 w-3 bg-green-500 rounded-full"></div>
                            </div>
                            <div class="space-y-2">
                                <div class="h-4 bg-slate-100 rounded w-3/4 animate-pulse"></div>
                                <div class="h-4 bg-slate-100 rounded w-full animate-pulse"></div>
                                <div class="h-4 bg-slate-100 rounded w-5/6 animate-pulse"></div>
                                <div class="mt-4 p-3 bg-slate-50 rounded text-xs font-mono text-slate-500">
                                    <span class="text-indigo-500">const</span> <span class="text-blue-600">developer</span> = {<br>
                                    &nbsp;&nbsp;name:<span class="text-green-600">'Muhammad Rigi Yuda Syahrial'</span>,<br>
                                    &nbsp;&nbsp;stack: [<span class="text-green-600">'Vue'</span>, <span class="text-green-600">'Laravel'</span>, <span class="text-green-600">'Tailwind CSS'</span>]<br>
                                };
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>