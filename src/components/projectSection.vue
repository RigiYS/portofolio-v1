<script setup>
import projectCard from './projectCard.vue';

const projects = [
    {
        title: "Larisin POS (Poin of Sales)",
        description: "Aplikasi kasir berbasis mobile untuk UMKM. Mengelola stok secara real-time, mencatat transaksi penjualan, dan menghasilkan laporan keuangan otomatis.",
        tags: ["React Native CLI", "Typescript", "CSS"],
        image: "https://www.soltius.co.id/site/uploads/images/5e2480cf5e14a-point-of-sales-software.jpg",
        repoLink: "https://github.com/RigiYS/larisin",
        demoLink: "#"
    },
    {
        title: "Sistem Informasi Perpustakaan",
        description: "Platform manajemen buku digital. Memungkinkan peminjaman, pengembalian, dan denda otomatis dengan validasi data yang ketat.",
        tags: ["PHP", "Bootstrap", "MySQL"],
        image: "https://images.unsplash.com/photo-1521587760476-6c12a4b040da?q=80&w=800&auto=format&fit=crop",
        repoLink: "-",
        demoLink: "-"
    },
    {
        title: "API Peminjaman Buku Online",
        description: "Backend Service (RESTful API) untuk sistem perpustakaan. Menangani autentikasi user dengan JWT, logika dengan otomatis, dan relasi database yang kompleks.",
        tags: ["Express.js", "Node.js", "MySQL", "JWT Auth"],
        image: "https://nusabot.id/blog/wp-content/uploads/2024/07/gabriel-heinzer-g5jpH62pwes-unsplash.jpg",
        repoLink: "-",
        demoLink: "-"
    },
]
</script>

<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <div class="text-center max-w-2xl mx-auto mb-16">
            <h2 class="text-3xl font-extrabold text-slate-900 mb-4">Featured Projects</h2>
            <p class="text-slate-600">
                Koleksi proyek pilihan yang menunjukkan kemampuan saya dalam membangun solusi <span class="text-indigo-600 font-bold">End-to-End</span>.
            </p>
        </div>

        <div class="grid grid-cols1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <projectCard v-for="(project, index) in projects" :key="index" v-bind="project"></projectCard>
        </div>

    </div>
</template>