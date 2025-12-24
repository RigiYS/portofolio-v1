<script setup>
const skills = [
    {
        category: "Front-End Development",
        items: ["Vue.js 3", "React", "Tailwind CSS", "HTML", "CSS", "JavaScript (ES6+)"]
    },
    {
        category: "Back-End Development",
        items: ["Node.js", "Express.js", "RESTful API Design"]
    },
    {
        category: "Database & Tools",
        items: ["MySQL", "Git/GitHub", "VS Code", "Postman"]
    },
];
</script>

<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid md:grid-cols-2 gap-12 items-center">

            <div data-aos="fade-up">
                <h2 class="text-3xl font-extrabold text-slate-900 mb-6">
                    About Me
                </h2>
                <div class="prose prose-lg text-slate-600 space-y-4">
                    <p>
                        A fifth-semester <strong>computer science</strong> student specializing in <strong>front-end development</strong>.
                    </p>
                    <p>
                        Experienced in building scalable web and mobile applications using <strong>React Native</strong>, <strong>Vue.js</strong>, and<strong> Node.js</strong>. I don't just write code; I focus on system efficiency and clean architecture.
                    </p>
                </div>

                <div class="mt-8 flex gap-8 border-t border-slate-200 pt-6">
                    <div>
                        <span class="block text-3xl font-bold text-indigo-600">5+</span>
                        <span class="text-sm text-slate-500 font-medium">Semester</span>
                    </div>
                    <div>
                        <span class="block text-3xl font-bold text-indigo-600">3+</span>
                        <span class="text-sm text-slate-500 font-medium">Major Projects</span>
                    </div>
                </div>
            </div>

            <div class="bg-white p-8 rounded-2xl shadow-xl border border-slate-100 relative overflow-hidden" data-aos="fade-up" data-aos-delay="200">
                <div class="absolute top-0 right-0 -mt-4 -mr-4 w-24 h-24 bg-indigo-50 rounded-full blur-xl opacity-50"></div>

                <h3 class="text-xl font-bold text-slate-900 mb-6 flex items-ceter gap-2">
                    <svg class="w-5 h-5 text-indigo-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path></svg>
                    Skills
                </h3>

                <div class="space-y-6">
                    <div v-for="(group, index) in skills" :key="index">
                        <h4 class="text-xs font-bold text-slate-400 uppercase tracking-wider mb-3">
                            {{ group.category  }}
                        </h4>
                        <div class="flex flex-wrap gap-2">
                            <span v-for="skill in group.items" :key="skill" class="px-3 py-1.5 bg-slate-50 text-slate-700 text-sm font-medium rounded-lg border border-slate-200 hover:border-idigo-300 hover:text-indigo-700 transition-colors cursor-default">
                                {{ skill }}
                            </span>
                        </div>
                    </div>
                </div>
            </div>
            
        </div>
    </div>
</template>