<script>
    import { page } from '$app/stores'
    import '../app.css'
  </script>
  
  <header class="fixed top-0 left-0 right-0 z-50 bg-background/80 backdrop-blur-sm border-b">
    <nav class="container mx-auto px-4 h-16 flex items-center justify-between">
      <a href="/" class="text-xl font-bold">Xian Rosario</a>
      <ul class="flex space-x-8">
        <li><a href="/" class="hover:text-primary {$page.url.pathname === '/' ? 'text-primary' : ''}">Home</a></li>
        <li><a href="/Portfolio-page" class="hover:text-primary {$page.url.pathname === '/Portfolio-page' ? 'text-primary' : ''}">Portfolio</a></li>
        <li><a href="/About-page" class="hover:text-primary {$page.url.pathname === '/About-page' ? 'text-primary' : ''}">About</a></li>
        <li><a href="/Contact-page" class="hover:text-primary {$page.url.pathname === '/Contact-page' ? 'text-primary' : ''}">Contact</a></li>
      </ul>
    </nav>
  </header>
  
  <main class="pt-24 min-h-screen">
    <slot />
  </main>
  
  <footer class="bg-muted py-8 mt-16">
    <div class="container mx-auto px-4 text-center">
      <p>©Xian Rosario {new Date().getFullYear()} Portfolio. All rights reserved.</p>
    </div>
  </footer>