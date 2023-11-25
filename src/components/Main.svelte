<script>
  import Step from "./Step.svelte";

  const steps = [
    {
      name: "Front-End Online Store",
      icon: "fa-solid fa-cart-shopping",
      href: "https://github.com/Netto-JM/frontend-online-store",
    },
    {
      name: "Back-End Soccer Management App",
      icon: "fa-solid fa-futbol",
      href: "https://github.com/Netto-JM/back-end-soccer-management-app",
    },
    {
      name: "Full-Stack Recipe App",
      icon: "fa-solid fa-utensils",
      href: "https://github.com/Netto-JM/recipe-app",
    },
  ]

    const benefits = [
      {
        name: "a self-taught developer",
        description: "I tought myself to code using both free online resources and some paid content"
      },
      {
        name: "someone who loves to learn",
        description: "I love learning new things and I'm always looking for new challenges and opportunities to grow and improve my skills."
      },
      {
        name: "someone who works well in a team",
        description: "I'm a team player and I'm always willing to help my teammates and learn from them."
      }
    ]
</script>

<main class="flex flex-col flex-1 p-4">
  <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi, I'm <span class="poppins text-violet-400">Juvenal</span> Martins <br />Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400">favorite tech</span> includes JavaScript or TypeScript (Vite or Next.js), 
        TailwindCSS, Node.js + Express & PostgreSQL, Java (17), Spring Ecosystem, Docker, MySQL
      </p>
      <a 
        href="mailto:nettojm86@gmail.com"
        target="_blank"
        class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins 
        relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
      >
        <div 
          class="absolute top-0 right-full w-full h-full bg-violet-400 
          opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9">Get in touch &rarr;</h4>
      </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img src={"images/profile.jpg"} alt="Profile" class="object-cover z-[2] max-h-[70vh]">
    </div>
  </section>


  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A few of my creative endeavors
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-violet-400">see</span> my work?
      </h3>
      
    </div>
    <a 
        href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
        target="_blank"
        class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex 
        items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
      >
        <i class="fa-regular fa-circle-play"></i>
        <p>Watch the video</p>
    </a>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p class="text-base sm:text-lg md:text-xl">
          Front-End Online Store is a <strong class="text-violet-400">React-based application</strong> that provides a simplified online shopping experience. 
          Users can explore a variety of products, add them to a shopping cart, and simulate the checkout process. 
          Leveraging the <strong class="text-violet-400">Mercado Livre API</strong>, the app allows for dynamic product searches and detailed product views, 
          making it a user-friendly front-end solution for online retail.
        </p>
      </Step>
      <Step step={steps[1]}>
        <p class="text-base sm:text-lg md:text-xl">
          This is a back-end soccer management app built with <strong class="text-violet-400">TypeScript, Node.js, Express.js,
          and Sequelize,</strong> designed to handle the management of soccer matches and team data. It provides authentication
          and offers a range of endpoints for creating, updating, and retrieving match and team information, making it a key component
          for a comprehensive soccer management system.
        </p>
      </Step>
      <Step step={steps[2]}>
        <p class="text-base sm:text-lg md:text-xl">
          The Full Stack Recipe App is a comprehensive platform developed with <strong class="text-violet-400">React</strong>
          on the front end and <strong class="text-violet-400">TypeScript, Node.js, Express.js, Sequelize, and Docker</strong>
          on the back end. It empowers users to explore, search, and manage a vast array of recipes for meals and drinks. 
          The app offers features like favoriting, progress tracking, and detailed recipe information. With its robust 
          front-end components and a dockerized back end, the Recipe App provides an engaging and efficient solution for 
          anyone passionate about cooking and trying new recipes.
        </p>
      </Step>
    </div>
  </section>
  <section id="about" class="py-20 pt-10 lg:py-32 lg:pt-16 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div 
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0
      before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute
      after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A little bit about me
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        <span class="poppins text-violet-400">Who</span> am I?
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am . . .
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
        <div class="flex gap-6 sm:gap-8">
          <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
            0{index + 1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <p class="text-base sm:text-lg md:text-xl">
              {benefit.description}
          </div>
        </div>
      {/each}
    </div>
    <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">The <span class="text-violet-400 poppins">Complete</span> Package</h5>
    <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
      <table class="bg-white text-slate-700 rounded text-center">
        <thead class="border-b border-solid border-slate-200">
          <tr>
            <th/>
            <th class="whitespace-nowrap py-2 px-4">Candidate #1</th>
            <th class="whitespace-nowrap py-2 px-4">Candidate #2</th>
            <th class="whitespace-nowrap py-2 px-4">Candidate #3</th>
            <th class="whitespace-nowrap bg-violet-700 text-white py-4 px-8">Me</th>
          </tr>
        </thead>
        <tbody>
          <tr class="border-b border-solid border-slate-200">
            <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">
              Dedication
            </td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check green-slate-500"></i></td>
          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">
              Critical Thinking
            </td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check green-slate-500"></i></td>
          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">
              Interpersonal Skills
            </td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-check green-slate-500"></i></td>
          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">
              Programming Ability
            </td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-check text-slate-500"></i></td>
            <td><i class="fa-solid fa-check green-slate-500"></i></td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
      <p>
        Scroll to see more &rarr;
      </p>
    </div>
    <p class="mx-auto">So why not invest?</p>
  </section>
</main>
