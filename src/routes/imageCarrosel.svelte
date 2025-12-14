<script lang="ts">
  import CarbonChevronLeft from "~icons/carbon/chevron-left";
  import CarbonChevronRight from "~icons/carbon/chevron-right";
  import { fade } from "svelte/transition";

  const images = [
    "https://www.w3schools.com/howto/img_nature_wide.jpg",
    "https://www.w3schools.com/howto/img_snow_wide.jpg",
    "https://www.w3schools.com/howto/img_lights_wide.jpg",
  ];

  let selectedIndex = 0;

  const subtractIndex = () => {
    if (selectedIndex - 1 >= 0) {
      selectedIndex--;
    }
  };

  const addIndex = () => {
    if (selectedIndex + 1 <= images.length - 1) {
      selectedIndex++;
    }
  };
</script>

<div class="w-full h-128 bg-gray-500 my-4 relative">
  {#each images as image, index}
    {#if index === selectedIndex}
      <img
        src={images[selectedIndex]}
        alt={images[selectedIndex]}
        class="w-full h-full"
        in:fade
      />
    {/if}
  {/each}
  <CarbonChevronLeft
    class="absolute top-1/2 left-4 text-4xl text-white cursor-pointer w-12 h-12 hover:bg-black/40 rounded-full flex justify-center items-center"
    onclick={subtractIndex}
  />
  <CarbonChevronRight
    class="absolute top-1/2 right-4 text-4xl text-white cursor-pointer w-12 h-12 hover:bg-black/40 rounded-full flex justify-center items-center"
    onclick={addIndex}
  />
</div>

<p class="text-center font-bold text-2xl">Conheça a</p>
<p class="text-center font-bold text-2xl">Clínica Budin</p>
