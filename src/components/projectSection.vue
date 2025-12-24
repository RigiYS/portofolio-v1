<script setup>
import projectCard from './projectCard.vue';

const projects = [
    {
        title: "Larisin POS (Point of Sales)",
        description: "Mobile-based cashier application for MSMEs. Manages stock in real-time, records sales transactions, and generates automatic financial reports.",
        tags: ["React Native CLI", "Typescript", "CSS"],
        image: "https://www.soltius.co.id/site/uploads/images/5e2480cf5e14a-point-of-sales-software.jpg",
        repoLink: "https://github.com/RigiYS/larisinApp",
        demoLink: "#"
    },
    {
        title: "Library Information System",
        description: "Digital book management platform. Enables borrowing, returning, and automatic fines with strict data validation.",
        tags: ["PHP", "Bootstrap", "MySQL"],
        image: "https://images.unsplash.com/photo-1521587760476-6c12a4b040da?q=80&w=800&auto=format&fit=crop",
        repoLink: "-",
        demoLink: "-"
    },
    {
        title: "API Lending Book Online",
        description: "Backend Service (RESTful API) for library systems. Handles user authentication with JWT, automated logic, and complex database relations.",
        tags: ["Express.js", "Node.js", "MySQL", "JWT Auth"],
        image: "https://nusabot.id/blog/wp-content/uploads/2024/07/gabriel-heinzer-g5jpH62pwes-unsplash.jpg",
        repoLink: "https://github.com/RigiYS/Library-Book-Lending-Online-API",
        demoLink: "-"
    },
]
</script>

<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <div class="text-center max-w-2xl mx-auto mb-16">
            <h2 class="text-3xl font-extrabold text-slate-900 mb-4">Projects</h2>
            <p class="text-slate-600">
                A curated collection of projects showcasing my ability to build <span class="text-indigo-600 font-bold">End-to-End</span> solutions.
            </p>
        </div>

        <div class="grid grid-cols1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <projectCard v-for="(project, index) in projects" :key="index" v-bind="project"></projectCard>
        </div>

    </div>
</template>