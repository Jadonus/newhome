<script lang="ts">
  import "../app.css";

  let bootstrap =
    "First of all, this is my opinion. Someone may think differently than me, and that is ok. Bootstrap is amazing for new web developers. It looks good out of the box. Check. It is Extremely good at making responsize websites. Check. It is accesable for everyone, with amazing documention and a massive userbase. Check. But here is where it goes wrong. Bootstrap is simply not customizable. Their color pallete is good, and with the semi recent release of Bootstrap 5, it has gotten better, but it does not have the flexibility like regular css. Don't get me wrong, I have some things to say about that too, but in regards to color, that is where regular css wins. In my opinion, what this website is built on uses what is the perfect balence between the two: Tailwind CSS. Tailwind still has a limited color pallete, but much less than Bootstrap. Tailwind's downside is no prebuilt items, like spinners, cards, buttons, etc. Instead of using the prebuilt items provided by Bootstrap, you get to make your own. This allows for flexibility and creativity at the expense of speed. I think that at the end of the day, Boostrap has its strengths, but Tailwind is my favorite. For now.";
  let bootstrap20 =
    "First of all, this is my opinion. Someone may think differently than me, and that is ok. Bootstrap";
</script>

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Poppins&display=swap"
  rel="stylesheet"
/>
<link href="https://fonts.cdnfonts.com/css/atakana-sarif" rel="stylesheet" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<div class="h-screen bg-purple-600">
  <h1
    class="pt-12 m-6 text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl"
  >
    In case you couldn't tell, I am inspired by <span
      class="dark:text-black text-white ani">minimalism</span
    >
  </h1>

  <p
    class="m-6 mt-4 text-xl sm:text-2xl md:text-2xl lg:text-2xl xl:text-2xl mb-24"
  >
    Websites should be easy to use and beautiful. So many of them fail miserably
    at this. My goal as a web developer is to be able to make the best websites
    possible.
  </p>
  <div class=" bg-purple-600 relative">
    <svg
      class="lg:m-24 xl:m-24 mt-12 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/4"
      xmlns="http://www.w3.org/2000/svg"
      version="1.1"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      xmlns:svgjs="http://svgjs.dev/svgjs"
      viewBox="250 250 350 325"
      ><defs
        ><radialGradient id="sssurface-grad-dark" r="75%" cx="20%" cy="20%">
          <stop offset="0%" stop-color="#000" stop-opacity="0" />
          <stop offset="100%" stop-color="#000000" stop-opacity="1" />
        </radialGradient><radialGradient
          id="sssurface-grad-light"
          r="25%"
          cx="30%"
          cy="30%"
        >
          <stop offset="0%" stop-color="#555555" stop-opacity="0.75" />
          <stop offset="100%" stop-color="#000" stop-opacity="0" />
        </radialGradient><filter
          id="sssurface-blur"
          x="-100%"
          y="-100%"
          width="400%"
          height="400%"
          filterUnits="objectBoundingBox"
          primitiveUnits="userSpaceOnUse"
          color-interpolation-filters="sRGB"
        >
          <feGaussianBlur
            stdDeviation="30"
            x="0%"
            y="0%"
            width="100%"
            height="100%"
            in="SourceGraphic"
            edgeMode="none"
            result="blur"
          /></filter
        ></defs
      ><g
        ><ellipse
          rx="150"
          ry="75"
          cx="450"
          cy="500"
          fill="#000000"
          opacity="0.25"
          filter="url(#sssurface-blur)"
        /><circle r="150" cx="400" cy="400" fill="#000000" /><circle
          r="150"
          cx="400"
          cy="400"
          fill="url(#sssurface-grad-dark)"
        /><circle
          r="150"
          cx="400"
          cy="400"
          fill="url(#sssurface-grad-light)"
        /></g
      ></svg
    >
  </div>
</div>

<body class="dark:bg-black dark:text-white antialiased">
  <main class="animate-fade-right p-4 sm:p-8 md:p-12 lg:p-16 xl:p-20">
    <h1
      class=" m-6 title text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl"
    >
      Who I am.
    </h1>
    <p
      class="mt-4 pb-24 text-xl sm:text-2xl md:text-3xl lg:text-4xl xl:text-5xl"
    >
      My name is Jadon, also known as Jadonus on various social media platforms.
      On this website, you will find my personal
      <a
        class="underline decoration-purple-500 hover:bg-purple-500 transition ease-in-out duration-300"
        href="/portfolio">portfolio</a
      >
      and
      <a
        class="underline decoration-purple-500 hover:bg-purple-500 transition ease-in-out duration-300"
        href="/blog">blog</a
      >. I am a full stack developer, with experience in Django, Wordpress, and
      Sveltekit. I am familiar with TailwindCSS and Bootstrap as well.
    </p>
  </main>

  <h1
    class="m-6 pt-16 title text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl"
  >
    Contact Me
  </h1>
    <form action="https://api.staticforms.xyz/submit" method="post">
     
<div class="m-12">
      <input
        class="m-2 dark:bg-black bg-white border-bottom border-b-4 mt-4 text-xl sm:text-2xl md:text-3xl lg:text-4xl xl:text-5x"
        type="text"
        name="name"
        placeholder="Your Name"
      /><br />

      <input
        class="m-2 dark:bg-black bg-white border-bottom border-b-4 mt-4 text-xl sm:text-2xl md:text-3xl lg:text-4xl xl:text-5x"
        type="text"
        name="email"
        placeholder="Your Email"
      /><br />
      <textarea
        class="dark:bg-black bg-white border-bottom border-b-4 mt-4 text-xl sm:text-2xl md:text-3xl lg:text-4xl xl:text-5x m-2"
        placeholder="Your Message"
        name="message"
      />
      <br />
      <input type="text" name="honeypot" style="display:none" />
      <input
        type="hidden"
        name="accessKey"
        value="9ffab3f9-26d8-4051-9398-bf8d4048744e"
      />
      <input type="hidden" name="subject" value="Contact Me!" />
      <input type="hidden" name="replyTo" value="@" />
      <input
        type="hidden"
        name="redirectTo"
        value="https://jadong.vercel.app"
      />
      <input
        class="bg-purple-600 rounded-lg p-2 mx-6"
        type="submit"
        value="Submit"
      />
    </form>

    <p class="">Made with ❤️ by Jadon Gearhart - 2023</p>
  </body
>

<style>
  main {
    font-family: "Poppins", sans-serif;
  }

  .title {
    font-family: "Atakana Sarif", Georgia;
  }

  @keyframes fade {
    0% {
      opacity: 0%;
    }
    100% {
      opacity: 100%;
    }
  }
  .ani {
    animation-name: fade;
    animation-duration: 2s;
    animation-iteration-count: infinite;
    animation-direction: alternate; /* This is the magical line! */
  }
</style>
