<script>
  import Step from "./Step.svelte";

  let step = [
    {
      name: "Spring Marketplace",
      icon: "fa-solid fa-store",
      href: "https://spring-marketplace-client.onrender.com/",
    },
    {
      name: "Pokedex",
      icon: "fa-solid fa-paw",
      href: "https://vanilla-pokedex.herokuapp.com/",
    },
    {
      name: "Texter Bot",
      icon: "fa-solid fa-message",
      href: "https://github.com/DMahyuddin/Texter-Bot",
    },
  ];
</script>

<main class="flex flex-col flex-1 p-4" id="introPage">
  <section class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div
      class="flex flex-col lg:jusify-center text-center lg:text-left gap-6 md:gap-8
      lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        <spam class="kanit text-waikawa-400">Dylan</spam> Mahyuddin
        <br /> Full Stack
        <spam class="kanit text-waikawa-400">Developer</spam>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        I'm a full stack Developer making anything that strikes interest.
      </p>
      <a
        href="https://www.linkedin.com/in/dylan-mahyuddin/"
        target="_blank"
        class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl kanit
         relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950
         cursor-pointer"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-waikawa-400 opacity-20
  group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9">Get in touch &rarr;</h4></a
      >
    </div>
  </section>
  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h3 class=" text-lg sm:text-xl md:text-2xl">
        <strong>Projects</strong>
      </h3>
      <!-- <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="kanit text-waikawa-400">see</span> my work?
      </h3> -->
    </div>
    <!-- <a
      href="https://github.com/DMahyuddin"
      target="_blank"
      class="mx-auto px-4 py-2 rounded-md border
    border-solid border-white flex item-center gap-2 -mb-4 sm:-mb-0
    -mt-10 hover:border-waikawa-700 duration-200"
      ><i class="fa-regular fa-circle-play" />
      <p>GitHub</p>
    </a> -->
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={step[0]}>
        <p>
          <strong class="text-waikawa-400">Springboot and Angular</strong>
          A group project to make a e-commerce website for farmers. They would be
          able to list produce and show off their food.
        </p></Step
      >
      <Step step={step[1]}>
        <p>
          <strong class="text-waikawa-400">HTML and JavaScript</strong>
          team project making a pokemon data search. grabs pokemon data from an API
          and displays it for the user.
        </p></Step
      >
      <Step step={step[2]}>
        <p>
          <strong class="text-waikawa-400">C#</strong> With the OpenAI api made a
          discord text bot to encode the users writing in other ways.
        </p></Step
      >
    </div>
  </section>
</main>
