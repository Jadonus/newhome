<script>
    import "../../app.css"
  
    let activeImage = null;
  
    // Function to open the full-screen image
    function openFullscreen(imageUrl) {
      activeImage = imageUrl;
    }
  
    // Function to close the full-screen image
    function closeFullscreen() {
      activeImage = null;
    }
  </script>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
  <link href="https://fonts.cdnfonts.com/css/atakana-sarif" rel="stylesheet">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
  <body class=" dark:bg-black dark:text-white antialiased">
    <main class="animate-fade-right p-4 sm:p-8 md:p-12 lg:p-16 xl:p-20">
      <a href="/"class="title text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl">Portfolio</a>
      <div class="text-xl sm:text-2xl md:text-3xl lg:text-4xl xl:text-5xl grid text-center gap-4 mt-12 grid-cols-1 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-3 grid-rows-3">
        <div>
          <a href="https://maverickjamespm.com"  class="underline decoration-purple-500 ease-in-out transition duration-400 hover:bg-purple-500">Maverick James Project Management Website</a>
          <p href="#" on:click={() => openFullscreen('mjpm.png')} class="mt-3">A website built for a client for their project management business. Made with a custom WordPress theme.</p>
        </div>
        <div>
          <a href="https://roadsbible.com" class="underline decoration-purple-500 ease-in-out transition duration-400 hover:bg-purple-500">Roads<br></a>
          <a href="#" on:click={() => openFullscreen('roads.png')} class="mt-3">A Bible memory app, built for simplicity and ease of use. Made with Django. </a>
        </div>
        <div>
          <a href="/" class="underline decoration-purple-500 ease-in-out transition duration-400 hover:bg-purple-500">This website<br></a>
          <a href="#" on:click={() => openFullscreen('s.png')} class="mt-3">Obviously you can see what this is. Made with SvelteKit.</a>
        </div>
      </div>
    
    </main>
  
    <!-- Display full-screen image if activeImage is not null -->
    {#if activeImage}
      <div class="fixed top-0 left-0 w-screen h-screen bg-black  flex items-center justify-center z-50">
        <img src={activeImage} alt="Full Screen Image" class="max-h-full max-w-full" on:click={closeFullscreen}>
      </div>
    {/if}
  </body>
  
  <style>
    main {
      font-family: 'Poppins', sans-serif;
    }
  
    
    /* Style for the full-screen image overlay */
    .fixed {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 9999;
    }
  
    img {
      max-width: 100%;
      max-height: 100%;
      cursor: pointer;
    }

::-webkit-scrollbar {
    display: none;
}
/* for Chrome */

  </style>
  
