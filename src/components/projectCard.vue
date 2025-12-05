<script setup>
defineProps({
  title: String,
  description: String,
  tags: Array,
  image: String,
  repoLink: String,
  demoLink: String
});
</script>

<template>
  <div class="group bg-white rounded-2xl border border-slate-100 overflow-hidden hover:shadow-xl hover:shadow-indigo-500/10 transition-all duration-300 flex flex-col h-full" data-aos="fade-up" data-aos-anchor-placement="top-bottom">
    
    <div class="h-48 w-full relative overflow-hidden bg-slate-100">
        <img 
          v-if="image" 
          :src="image" 
          :alt="title" 
          class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110"
        />
        
        <div v-else class="w-full h-full flex items-center justify-center bg-indigo-50 text-4xl">
            💻
        </div>

        <div class="absolute inset-0 bg-indigo-900/0 group-hover:bg-indigo-900/10 transition-colors duration-300"></div>
    </div>

    <div class="p-6 flex flex-col flex-grow">
      
      <div class="flex justify-between items-start mb-4">
        <h3 class="text-xl font-bold text-slate-900 leading-tight group-hover:text-indigo-600 transition-colors">
          {{ title }}
        </h3>
        <a :href="repoLink" target="_blank" class="text-slate-400 hover:text-indigo-600 transition-colors">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m-6-6L10 14"></path></svg>
        </a>
      </div>

      <p class="text-slate-600 text-sm mb-6 flex-grow leading-relaxed">
        {{ description }}
      </p>

      <div class="flex flex-wrap gap-2 mt-auto">
        <span v-for="tag in tags" :key="tag" 
          class="px-2.5 py-1 text-xs font-semibold text-slate-600 bg-slate-100 rounded-md border border-slate-200">
          {{ tag }}
        </span>
      </div>

      <div class="mt-6 pt-4 border-t border-slate-100 flex gap-4">
         <a v-if="repoLink" :href="repoLink" target="_blank" class="text-sm font-bold text-slate-700 hover:text-indigo-600 flex items-center gap-1">
            <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.477 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .26.18.57.688.475A10.005 10.005 0 0122 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" /></svg>
            Source Code
         </a>
      </div>

    </div>
  </div>
</template>