<script>
    const socialLinks = [
      {
        platform: "GitHub",
        url: "https://github.com/xianrosario",
        icon: "github"
      },
      {
        platform: "Instagram",
        url: "https://www.instagram.com/yaaaangying_/",
        icon: "Instagram"
      },
      {
        platform: "Twitter",
        url: "https://x.com/yangxrosario",
        icon: "twitter"
      }
    ]
  </script>
  
  <div class="container mx-auto px-4 max-w-2xl">
    <h1 class="text-4xl font-bold mb-8">Contact Me</h1>
    
    <div class="bg-card rounded-lg p-6 shadow-lg">
      <h2 class="text-2xl font-semibold mb-4">Get in Touch</h2>
      
      <form class="space-y-4">
        <div>
          <label for="name" class="block text-sm font-medium mb-1">Name</label>
          <input
            type="text"
            id="name"
            class="w-full p-2 rounded-md border bg-background"
            required
          />
        </div>
        
        <div>
          <label for="email" class="block text-sm font-medium mb-1">Email</label>
          <input
            type="email"
            id="email"
            class="w-full p-2 rounded-md border bg-background"
            required
          />
        </div>
        
        <div>
          <label for="message" class="block text-sm font-medium mb-1">Message</label>
          <textarea
            id="message"
            rows="4"
            class="w-full p-2 rounded-md border bg-background"
            required
          ></textarea>
        </div>
        
        <button
          type="submit"
          class="w-full bg-primary text-primary-foreground py-2 rounded-md hover:opacity-90 transition-opacity"
        >
          Send Message
        </button>
      </form>
      
      <div class="mt-8">
        <h2 class="text-xl font-semibold mb-4">Connect with Me</h2>
        <div class="flex gap-4">
          {#each socialLinks as link}
            <a
              href={link.url}
              class="text-muted-foreground hover:text-primary transition-colors"
              target="_blank"
              rel="noopener noreferrer"
            >
              {link.platform}
            </a>
          {/each}
        </div>
        
        <div class="mt-4">
          <p class="text-muted-foreground">
            Email: <a href="mailto:your.email@example.com" class="text-primary hover:underline">202211990@gordoncollege.edu.ph</a>
          </p>
        </div>
      </div>
    </div>
  </div>