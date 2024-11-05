<script>
    const projects = [

      {
        title: "Portfoilio",
        description: "My portfolio site made with SvelteKit and Tailwind CSS, showcasing my projects with a clean, responsive design.",
        image: 'assets/portfolio-image.jpg',
        github: "https://github.com/xianrosario/xianrosario.github.io",
      },

    ]
  </script>
  
  <div class="container mx-auto px-4">
    <h1 class="text-4xl font-bold mb-8">My Portfolio</h1>
    
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      {#each projects as project}
        <article class="border rounded-lg overflow-hidden hover:shadow-lg transition-shadow">
          <img 
            src={project.image} 
            alt={project.title}
            class="w-full h-48 object-cover"
            width="400"
            height="200"
          />
          <div class="p-4">
            <h2 class="text-xl font-semibold mb-2">{project.title}</h2>
            <p class="text-muted-foreground mb-4">{project.description}</p>
            <div class="flex gap-4">
              <a 
                href={project.github}
                class="text-sm text-primary hover:underline"
                target="_blank"
                rel="noopener noreferrer"
              >
                GitHub
              </a>
            </div>
          </div>
        </article>
      {/each}
    </div>
  </div>