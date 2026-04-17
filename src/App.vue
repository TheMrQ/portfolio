<script setup>
import { onMounted } from 'vue';

onMounted(() => {
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.remove('opacity-0', 'translate-y-12');
        entry.target.classList.add('opacity-100', 'translate-y-0');
      } else {
        entry.target.classList.remove('opacity-100', 'translate-y-0');
        entry.target.classList.add('opacity-0', 'translate-y-12');
      }
    });
  }, {
    threshold: 0.15,
    rootMargin: "0px 0px -50px 0px"
  });

  document.querySelectorAll('.reveal-target').forEach((el) => {
    observer.observe(el);
  });
});
</script>

<template>
  <div class="min-h-screen bg-slate-50 text-slate-800 font-sans selection:bg-purple-200 overflow-x-hidden">
    
    <nav class="sticky top-0 z-50 bg-white/70 backdrop-blur-lg border-b border-slate-200/50">
      <div class="max-w-5xl mx-auto px-6 py-4 flex justify-between items-center">
        <div class="font-black text-2xl tracking-tighter bg-gradient-to-r from-indigo-600 to-pink-500 text-transparent bg-clip-text">Portfolio.</div>
        <div class="space-x-6 text-sm font-semibold flex items-center text-slate-600">
          <a href="#about" class="hover:text-indigo-600 transition-colors hidden sm:block">About</a>
          <a href="#projects" class="hover:text-indigo-600 transition-colors hidden sm:block">Projects</a>
          <a href="#contact" class="hover:text-indigo-600 transition-colors">Contact</a>
          <a href="https://github.com/TheMrQ" target="_blank" class="flex items-center px-4 py-2 bg-slate-900 text-white rounded-full hover:bg-slate-800 transition-all hover:-translate-y-0.5 hover:shadow-md">
            <svg class="w-4 h-4 mr-2" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
              <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" />
            </svg>
            GitHub
          </a>
        </div>
      </div>
    </nav>

    <header class="relative overflow-hidden bg-[radial-gradient(#e2e8f0_1px,transparent_1px)] [background-size:24px_24px]">
      <div class="absolute inset-0 bg-gradient-to-b from-transparent to-slate-50"></div>
      <div class="max-w-5xl mx-auto px-6 py-20 md:py-32 relative z-10 flex flex-col-reverse md:flex-row items-center gap-16">
        
        <div class="flex-1 reveal-target opacity-0 translate-y-12 transition-all duration-1000 ease-out">
          <div class="inline-block px-4 py-1.5 rounded-full bg-indigo-50 border border-indigo-100 text-indigo-600 font-bold text-sm mb-6 tracking-wide uppercase shadow-sm">
            Available for opportunities
          </div>
          <h1 class="text-5xl md:text-6xl font-extrabold tracking-tight text-slate-900 mb-6 leading-[1.1]">
            Hi, I'm <span class="text-indigo-600">Tuấn Quỳnh</span>. <br class="hidden md:block" />
            I build <span class="text-transparent bg-clip-text bg-gradient-to-r from-indigo-600 via-purple-600 to-pink-500">modern applications.</span>
          </h1>
          <p class="text-lg md:text-xl text-slate-600 max-w-2xl mb-10 leading-relaxed font-medium">
            I'm in my final year at Can Tho University. I enjoy working across the stack and specialize in a diverse range of languages to solve problems and create seamless, beautiful user experiences.
          </p>

          <div class="flex flex-wrap gap-3 max-w-3xl">
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/csharp/csharp-original.svg" class="w-4 h-4 mr-2" alt="C#" /> C#
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" class="w-4 h-4 mr-2" alt="HTML5" /> HTML5
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" class="w-4 h-4 mr-2" alt="CSS3" /> CSS3
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" class="w-4 h-4 mr-2" alt="JavaScript" /> JavaScript
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" class="w-4 h-4 mr-2" alt="Vue.js" /> Vue.js
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" class="w-4 h-4 mr-2" alt="PHP" /> PHP
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" class="w-4 h-4 mr-2" alt="MySQL" /> MySQL
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" class="w-4 h-4 mr-2" alt="Python" /> Python
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" class="w-4 h-4 mr-2" alt="Java" /> Java
            </span>
            <span class="flex items-center px-3 py-2 bg-white text-slate-700 text-sm font-bold rounded-lg border border-slate-200 shadow-sm hover:shadow-md hover:-translate-y-1 hover:border-indigo-300 transition-all cursor-default">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" class="w-4 h-4 mr-2" alt="Figma" /> Figma
            </span>
          </div>
        </div>
        
        <div class="relative group reveal-target opacity-0 translate-y-12 transition-all duration-1000 delay-200 ease-out">
          <div class="absolute -inset-1 bg-gradient-to-r from-indigo-500 to-pink-500 rounded-full blur opacity-25 group-hover:opacity-50 transition duration-1000 group-hover:duration-200"></div>
          <div class="relative w-56 h-56 md:w-72 md:h-72 shrink-0 rounded-full overflow-hidden border-4 border-white shadow-2xl">
            <img src="./assets/IMG_1899.jpg" alt="Profile Picture" class="w-full h-full object-cover object-top hover:scale-105 transition-transform duration-700" />
          </div>
        </div>
      </div>
    </header>

    <section id="about" class="bg-indigo-50/50">
      <div class="max-w-5xl mx-auto px-6 py-24">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-16">
          
          <div class="bg-white p-8 rounded-2xl border border-slate-100 hover:shadow-md reveal-target opacity-0 translate-y-12 transition-all duration-1000 ease-out">
            <div class="flex items-center mb-6">
              <div class="w-12 h-12 rounded-xl bg-indigo-100 flex items-center justify-center text-indigo-600 mr-4 shadow-inner">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 00-3.09 3.09zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456zM16.894 20.567L16.5 21.75l-.394-1.183a2.25 2.25 0 00-1.423-1.423L13.5 18.75l1.183-.394a2.25 2.25 0 001.423-1.423l.394-1.183.394 1.183a2.25 2.25 0 001.423 1.423l1.183.394-1.183.394a2.25 2.25 0 00-1.423 1.423z" />
                </svg>
              </div>
              <h2 class="text-2xl font-bold text-slate-900">Technical Strengths</h2>
            </div>
            <div class="space-y-4 text-slate-600 text-base leading-relaxed">
              <p>
                <strong class="text-indigo-900">Aesthetic-Driven Engineering:</strong> I have a strong focus on the intersection of logic and design. Beyond just writing functional code, I possess a keen eye for UI/UX principles, ensuring that the interfaces I build are highly polished, modern, and intuitive.
              </p>
              <p>
                <strong class="text-indigo-900">Adaptable Problem Solving:</strong> From setting up backend databases to perfecting front-end responsive layouts, I love bridging the gap between infrastructure and a beautiful user experience.
              </p>
            </div>
          </div>
          
          <div class="bg-white p-8 rounded-2xl border border-slate-100 hover:shadow-md reveal-target opacity-0 translate-y-12 transition-all duration-1000 delay-200 ease-out">
            <div class="flex items-center mb-6">
              <div class="w-12 h-12 rounded-xl bg-pink-100 flex items-center justify-center text-pink-600 mr-4 shadow-inner">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M9.53 16.122a3 3 0 00-5.965 1.178c.033.4.296.726.68.868.5.187 1.05.292 1.625.292s1.125-.105 1.625-.292c.384-.142.647-.468.68-.868a3 3 0 00-1.645-3.178zM15 12a3 3 0 100-6 3 3 0 000 6z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12c0-5.385 4.365-9.75 9.75-9.75s9.75 4.365 9.75 9.75-4.365 9.75-9.75 9.75S2.25 17.385 2.25 12zm13.36-1.814a6.368 6.368 0 01-1.113-1.113M12 15a3 3 0 11-6 0 3 3 0 016 0z" />
                </svg>
              </div>
              <h2 class="text-2xl font-bold text-slate-900">Beyond the Code</h2>
            </div>
            <div class="space-y-4 text-slate-600 text-base leading-relaxed">
              <p>
                I believe that drawing inspiration from different areas of life fuels better problem-solving. I'm a creative at heart, so you can often find me working on digital art—sketching and coloring character illustrations. 
              </p>
              <p>
                I'm also incredibly passionate about discovering and playing music. To stay active and balanced, I regularly head out to the field to play soccer, which constantly reminds me of the value of quick teamwork outside the IDE.
              </p>
            </div>
          </div>

        </div>
      </div>
    </section>

    <section id="projects" class="bg-white">
      <div class="max-w-5xl mx-auto px-6 py-24">
        
        <div class="flex items-center justify-between mb-12 reveal-target opacity-0 translate-y-12 transition-all duration-1000 ease-out">
          <h2 class="text-4xl font-extrabold text-slate-900 tracking-tight">Featured Work</h2>
          <div class="h-1 flex-grow bg-gradient-to-r from-indigo-100 to-transparent ml-8 rounded-full hidden sm:block"></div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-12 md:gap-16">
          
          <div class="group flex flex-col reveal-target opacity-0 translate-y-12 transition-all duration-1000 ease-out">
            <div class="bg-slate-100 aspect-video rounded-2xl mb-6 overflow-hidden border border-slate-200 relative shadow-md group-hover:shadow-xl group-hover:-translate-y-2 transition-all duration-300">
              <img src="./assets/animac-preview.png" alt="Animac Tracker Preview" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
              <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
            </div>
            
            <h3 class="text-2xl font-bold text-slate-900 mb-3 group-hover:text-indigo-600 transition-colors">Animac Tracker</h3>
            <p class="text-slate-600 mb-6 flex-grow leading-relaxed">
              A fully responsive anime tracking platform. Designed with a mobile-first approach to ensure a flawless experience across all devices, including strict iOS layout standards.
            </p>
            <div class="flex items-center space-x-4">
              <a href="https://animac.site" target="_blank" class="inline-flex items-center px-5 py-2.5 bg-indigo-50 text-indigo-700 font-bold rounded-full hover:bg-indigo-600 hover:text-white transition-all shadow-sm">
                View Live Site 
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-4 h-4 ml-2">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 6H5.25A2.25 2.25 0 003 8.25v10.5A2.25 2.25 0 005.25 21h10.5A2.25 2.25 0 0018 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25" />
                </svg>
              </a>
            </div>
          </div>

          <div class="group flex flex-col reveal-target opacity-0 translate-y-12 transition-all duration-1000 delay-200 ease-out">
            <div class="bg-slate-100 aspect-video rounded-2xl mb-6 overflow-hidden border border-slate-200 relative shadow-md group-hover:shadow-xl group-hover:-translate-y-2 transition-all duration-300">
              <img src="./assets/image.png" alt="Zenith Preview" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
              <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
            </div>
            <h3 class="text-2xl font-bold text-slate-900 mb-3 group-hover:text-pink-600 transition-colors">Zenith</h3>
            <p class="text-slate-600 mb-6 flex-grow leading-relaxed">
              A hosted financial tracking application utilizing SQLi and a PHP backend to securely and efficiently manage daily expenses.
            </p>
            <div class="flex items-center space-x-4">
               <a href="http://expense-manager-api.42web.io" target="_blank" class="inline-flex items-center px-5 py-2.5 bg-pink-50 text-pink-700 font-bold rounded-full hover:bg-pink-600 hover:text-white transition-all shadow-sm">
                View Live Site
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-4 h-4 ml-2">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 6H5.25A2.25 2.25 0 003 8.25v10.5A2.25 2.25 0 005.25 21h10.5A2.25 2.25 0 0018 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25" />
                </svg>
              </a>
            </div>
          </div>

        </div>
      </div>
    </section>

    <section id="contact" class="bg-indigo-50/30 border-t border-indigo-100/50">
      <div class="max-w-4xl mx-auto px-6 py-24 text-center">
        <div class="reveal-target opacity-0 translate-y-12 transition-all duration-1000 ease-out">
          <h2 class="text-4xl font-extrabold text-slate-900 mb-6">Let's Connect</h2>
          <p class="text-lg text-slate-600 max-w-2xl mx-auto mb-10 leading-relaxed">
            I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision. 
          </p>
          
          <div class="flex flex-col sm:flex-row items-center justify-center gap-6 mb-12">
            <a href="mailto:tuanquynhlol@gmail.com" class="inline-flex items-center justify-center px-8 py-3.5 text-base font-bold text-white transition-all bg-indigo-600 rounded-full shadow-sm hover:bg-indigo-700 hover:shadow-md hover:-translate-y-1">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5 mr-2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
              </svg>
              Drop me an email
            </a>
          </div>

          <div class="flex flex-wrap items-center justify-center gap-8 text-slate-600 font-medium">
            <div class="flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 mr-2 text-indigo-500">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z" />
              </svg>
              Dong Thap
            </div>
            <a href="https://github.com/TheMrQ" target="_blank" class="flex items-center hover:text-indigo-600 transition-colors">
              <svg class="w-5 h-5 mr-2 text-indigo-500" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" />
              </svg>
              GitHub
            </a>
          </div>
        </div>
      </div>
    </section>

    <footer class="bg-slate-50 border-t border-slate-200 py-12 text-center text-slate-500 text-sm font-medium">
      <div class="max-w-5xl mx-auto px-6 flex flex-col items-center justify-center">
        <div class="w-8 h-8 mb-4 bg-gradient-to-br from-indigo-500 to-pink-500 rounded-lg flex items-center justify-center text-white font-bold shadow-sm">
          P.
        </div>
        <p>© {{ new Date().getFullYear() }} — Built with Vue.js & Tailwind CSS.</p>
      </div>
    </footer>
  </div>
</template>

<style>
html {
  scroll-behavior: smooth;
}
</style>