<script>
  import SectionWrapper from "./SectionWrapper.svelte"
  import Header from "./Header.svelte"
  import CtAs from "./CTAs.svelte";
</script>


<SectionWrapper>
  <Header />
  <div class="flex flex-col gap-10 flex-1 items-center justify-center pd-10 md:pd-14">
    <h2 class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl max-w-[1200px] mx-auto w-full text-center font-semibold">
      <span class="text-indigo-400">Gym</span> 
      Training <span class="text-indigo-600 line-through">Is Hard</span><br>
      Just Got <span class="text-indigo-400">Easier</span>
    </h2>
    <p class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] mx-auto w-full">
      Less thinking & more doing. We're the trainer in your pocket
      full of <span class="italic">
        personalized workouts, excercise and explanations, analytics
      </span>
      and much much more.
    </p>
    <CtAs />
    <div class="flex items-center justify-center gap-2 text-base">
      <p>4.6</p>
      {#each [0,1,2,3,4] as index}
      <div class="grid place-items-center relative">
        <i class="fa-solid fa-star opacity-0"></i>
      </div>
      {/each}
    </div>
  </div>
</SectionWrapper>