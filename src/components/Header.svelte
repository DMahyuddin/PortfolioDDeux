<script>
  export let y;

  let tabs = [
    { name: "About me", link: "#introPage" },
    { name: "Projects", link: "#projects" },
    { name: "Links", link: "#links" },
  ];
</script>

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid " +
    (y > 0
      ? " py-4 bg-waikawa-950 border-waikawa-700 rounded-lg"
      : "py-6 bg-transparent border-transparent ")}
>
  <h1 class="font-medium"><b class="font-bold kanit">Dylan</b> Mahyuddin</h1>
  <div class="sm:flex items-center gap-4 hidden">
    {#each tabs as tab, index}
      <a href={tab.link} class="duration-200 hover:text-waikawa-400">
        <p>{tab.name}</p>
      </a>
    {/each}
    <a
      href="https://www.linkedin.com/in/dylan-mahyuddin/"
      target="_blank"
      class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white
  text-waikawa-950"
    >
      <div
        class="absolute top-0 right-full w-full h-full bg-waikawa-400 opacity-20
group-hover:translate-x-full z-0 duration-200"
      />
      <h4 class="relative z-9">Get in touch</h4></a
    >
  </div>
</header>
