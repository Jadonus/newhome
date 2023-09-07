<script lang="ts">
    import { page } from '$app/stores';
    import { onMount } from 'svelte';
    import { writable } from 'svelte/store'; // Import writable store
    import "../../../app.css";

    // Define your blogs
    let blogs = {
      bootstrap: `
        First of all, this is my opinion. Someone may think differently than me, and that is ok. Bootstrap is amazing for new web developers. It looks good out of the box. Check. It is Extremely good at making responsize websites. Check. It is accesable for everyone, with amazing documention and a massive userbase. Check. But here is where it goes wrong. Bootstrap is simply not customizable. Their color pallete is good, and with the semi recent release of Bootstrap 5, it has gotten better, but it does not have the flexibility like regular css. Don't get me wrong, I have some things to say about that too, but in regards to color, that is where regular css wins. In my opinion, what this website is built on uses what is the perfect balence between the two: Tailwind CSS. Tailwind still has a limited color pallete, but much less than Bootstrap. Tailwind's downside is no prebuilt items, like spinners, cards, buttons, etc. Instead of using the prebuilt items provided by Bootstrap, you get to make your own. This allows for flexibility and creativity at the expense of speed. I think that at the end of the day, Boostrap has its strengths, but Tailwind is my favorite. For now....
      `,
      hello: `
Hello. I dont know why I wrote this, but still, Hello. 
By the way, Hello.
      `
    };
  
    // Create a writable store for currentBlog
    const currentBlog = writable("Select a blog from the menu"); // Provide a default value
  
    onMount(async () => {
      // Access the value of `page` store inside `onMount`
      const slug = $page.params.slug; // Get the slug from the URL
      if (slug in blogs) {
        currentBlog.set(blogs[slug]); // Set the corresponding blog content if the slug exists
      } else {
        currentBlog.set("Blog not found"); // Set a message if the slug doesn't match any blogs
      }
    });
  </script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
<link href="https://fonts.cdnfonts.com/css/atakana-sarif" rel="stylesheet">
 <body class=" dark:bg-black h-screen dark:text-white antialiased">
  <!-- The rest of your HTML -->
  <main class="animate-fade-right p-4 sm:p-8 md:p-12 lg:p-16 xl:p-20">
    <h1 class="m-6 title text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl"> {$page.params.slug}</h1>
    <div class="hello mt-4 text-xl sm:text-xl md:text-xl lg:text-2xl xl:text-3xl">
      {$currentBlog}
    </div>
  
  </main>
  </body>
<style>
        .hello {
            font-family: 'Poppins', sans-serif;
        }

        .title {
            font-family: 'Atakana Sarif', Georgia;
        }
    </style>
