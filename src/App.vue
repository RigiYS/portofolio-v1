<script setup>
import Navbar from './components/navbar.vue';
import heroSection from './components/heroSection.vue';
import aboutSection from './components/aboutSection.vue';
import projectSection from './components/projectSection.vue';
import Footer from './components/footer.vue';
</script>

<template>
  <div class="bg-slate-50 min-h-screen font-sans text-slate-800">

    <Navbar />

    <main>
      <section id="home">
        <heroSection />
      </section>

      <section id="about" class="py-24 bg-white relative">
        <aboutSection />
      </section>

      <section id="projects" class="py-24 bg-slate-50 border-t border-slate-200">
        <projectSection />
      </section>
    </main>    

    <Footer />

  </div>
</template>