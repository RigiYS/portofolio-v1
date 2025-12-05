<script setup>
const socialLinks = [
    {
        name: 'GitHub',
        href: 'https://github.com/RigiYS', 
        icon: 'M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.477 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .26.18.57.688.475A10.005 10.005 0 0122 12.017C22 6.484 17.522 2 12 2z'
    },
    {
        name: 'Email',
        href: 'mailto:rigiyuda123@gmail.com',
        icon: 'M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z'
    },
    {
        name: 'Whatsapp',
        href: 'https://wa.me/+6281385605396',
        icon: 'M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z'
    }
];

const currentYear = new Date().getFullYear();
</script>

<template>
    <footer class="bg-slate-900 text-slate-300 py-12 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

            <div class="flex flex-col md:flex-row justify-between items-center gap-8">

                <div class="text-center md:text-left">
                    <h2 class="text-2xl font-bold text-white tracking-tighter mb-2">
                        Rigi<span class="text-indigo-500">.Dev</span>
                    </h2>
                    <p class="text-sm text-slate-400 max-w-xs">
                        Membangun solusi digital yang andal dengan fokus pada performa dan pengalaman pengguna.
                    </p>
                </div>

                <div class="flex space-x-6">
                    <a v-for="item in socialLinks" :key="item.name" :href="item.href" target="_blank"
                        class="text-slate-400 hover:text-white hover:scale-110 transition-all duration-300">
                        <span class="sr-only">{{ item.name }}</span>
                        <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                            <path :d="item.icon" />
                        </svg>
                    </a>
                </div>

            </div>

            <div class="border-t border-slate-800 my-8"></div>

            <div class="flex flex-col md:flex-row justify-between items-center text-sm text-slate-500">
                <p>&copy; {{ currentYear }} Muhammad Rigi Yuda Syahrial. All rights reserved.</p>
                <p class="mt-2 md:mt-0 flex items-center gap-1">
                    Built with
                    <span class="text-green-500 font-bold">Vue</span> and
                    <span class="text-sky-500 font-bold">Tailwind CSS</span>
                </p>
            </div>

        </div>
    </footer>
</template>