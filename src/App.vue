<template>
  <div class="min-h-screen bg-slate-50 text-slate-800 font-sans selection:bg-blue-200">
    
    <nav class="sticky top-0 z-50 bg-white/80 backdrop-blur-md border-b border-slate-200">
      <div class="max-w-5xl mx-auto px-6 py-5 flex justify-between items-center">
        <div class="font-bold text-xl tracking-tight text-slate-900">Portfolio.</div>
        <div class="space-x-6 text-sm font-medium flex items-center">
          <a href="#projects" class="hover:text-blue-600 transition-colors">Projects</a>
          <a href="https://github.com/TheMrQ" target="_blank" class="flex items-center hover:text-blue-600 transition-colors">
            <svg class="w-5 h-5 mr-1.5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
              <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" />
            </svg>
            GitHub
          </a>
        </div>
      </div>
    </nav>

    <header class="relative border-b border-slate-200 bg-[radial-gradient(#e2e8f0_1px,transparent_1px)] [background-size:24px_24px]">
      <div class="max-w-5xl mx-auto px-6 py-20 md:py-32 relative z-10">
        <h1 class="text-5xl md:text-6xl font-extrabold tracking-tight text-slate-900 mb-6 leading-tight bg-white/70 inline-block pr-4 rounded-lg">
          Hi, I'm an IT student <br class="hidden md:block" /> building modern applications.
        </h1>
        <p class="text-lg md:text-xl text-slate-700 max-w-2xl mb-8 leading-relaxed bg-white/80 p-2 rounded-lg backdrop-blur-sm">
          I'm in my final year at Can Tho University. I enjoy working across the stack and specialize in a diverse range of languages and tools to solve problems and create seamless user experiences.
        </p>

        <div class="flex flex-wrap gap-3 mb-10 max-w-3xl">
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/csharp/csharp-original.svg" class="w-4 h-4 mr-2" alt="C#" /> C#
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" class="w-4 h-4 mr-2" alt="HTML5" /> HTML5
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" class="w-4 h-4 mr-2" alt="CSS3" /> CSS3
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" class="w-4 h-4 mr-2" alt="JavaScript" /> JavaScript
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" class="w-4 h-4 mr-2" alt="Vue.js" /> Vue.js
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg" class="w-4 h-4 mr-2" alt="PHP" /> PHP
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" class="w-4 h-4 mr-2" alt="MySQL" /> MySQL
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" class="w-4 h-4 mr-2" alt="Python" /> Python
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" class="w-4 h-4 mr-2" alt="Java" /> Java
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/dart/dart-original.svg" class="w-4 h-4 mr-2" alt="Dart" /> Dart
          </span>
          <span class="flex items-center px-3 py-1.5 bg-white text-slate-700 text-sm font-semibold rounded-md border border-slate-200 shadow-sm hover:border-slate-300 transition-colors">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/figma/figma-original.svg" class="w-4 h-4 mr-2" alt="Figma" /> Figma
          </span>
        </div>

        <a href="mailto:YOUR_EMAIL@EXAMPLE.COM" class="inline-flex items-center bg-blue-600 text-white px-8 py-3 rounded-full font-semibold hover:bg-blue-700 transition-all shadow-md hover:shadow-lg hover:-translate-y-0.5">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5 mr-2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
          </svg>
          Get in touch
        </a>
      </div>
    </header>

    <section id="projects" class="bg-white">
      <div class="max-w-5xl mx-auto px-6 py-20">
        <div class="flex items-center mb-12">
          <h2 class="text-3xl font-bold text-slate-900 pr-6">Featured Work</h2>
          <div class="flex-grow h-px bg-slate-200"></div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
          
          <div class="group">
            <div class="bg-slate-100 aspect-video rounded-xl mb-6 overflow-hidden border border-slate-200 relative shadow-sm">
              <img src="./assets/animac-preview.png" alt="Animac Tracker Preview" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
            </div>
            
            <h3 class="text-2xl font-bold text-slate-900 mb-2">Animac Tracker</h3>
            <p class="text-slate-600 mb-4 line-clamp-3">
              A fully responsive anime tracking platform. Designed with a mobile-first approach to ensure a flawless experience across all devices, including strict iOS layout standards.
            </p>
            <div class="flex items-center space-x-4">
              <a href="https://animac.site" target="_blank" class="inline-flex items-center text-blue-600 font-semibold hover:text-blue-800 transition-colors">
                View Live Site 
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor" class="w-4 h-4 ml-1">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 6H5.25A2.25 2.25 0 003 8.25v10.5A2.25 2.25 0 005.25 21h10.5A2.25 2.25 0 0018 18.75V10.5m-10.5 6L21 3m0 0h-5.25M21 3v5.25" />
                </svg>
              </a>
            </div>
          </div>

          <div class="group">
            <div class="bg-slate-900 aspect-video rounded-xl mb-6 overflow-hidden border border-slate-800 p-8 shadow-sm flex flex-col justify-center relative transition-transform duration-500 group-hover:-translate-y-1 group-hover:shadow-lg">
               <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-8 h-8 text-blue-400 mb-4 absolute top-6 right-6 opacity-30">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 6.75L22.5 12l-5.25 5.25m-10.5 0L1.5 12l5.25-5.25m7.5-3l-4.5 16.5" />
               </svg>
               <h4 class="text-blue-400 font-mono text-sm mb-3"># Database Migration</h4>
               <p class="text-slate-200 font-medium leading-relaxed text-lg z-10">Refactored legacy SQLi codebase to secure PDO, eliminating injection vulnerabilities.</p>
            </div>
            <h3 class="text-2xl font-bold text-slate-900 mb-2">Expense Manager</h3>
            <p class="text-slate-600 mb-4">
              A financial tracking application highlighting backend security. Led the migration of the database connectivity from standard SQLi to robust PDO prepared statements.
            </p>
            <div class="flex items-center space-x-4">
               <a href="#" class="inline-flex items-center text-slate-600 font-semibold hover:text-slate-900 transition-colors">
                <svg class="w-4 h-4 mr-1.5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                  <path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z" clip-rule="evenodd" />
                </svg>
                View GitHub Repo
              </a>
            </div>
          </div>

        </div>
      </div>
    </section>

    <footer class="bg-slate-50 border-t border-slate-200 py-12 text-center text-slate-500 text-sm">
      <div class="max-w-5xl mx-auto px-6">
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