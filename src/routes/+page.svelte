<script lang="ts">
  import AboutTheClinic from "./AboutTheClinic.svelte";
  import FAQ from "./FAQ.svelte";
  import Footer from "./Footer.svelte";
  import GoogleAvaliations from "./GoogleAvaliations.svelte";
  import Header from "./Header.svelte";
  import ImageCarrosel from "./imageCarrosel.svelte";
  import Main from "./Main.svelte";
  import Services from "./Services.svelte";
  import WhyChoose from "./WhyChoose.svelte";

  // let scroll: number;
</script>

<!-- <svelte:window bind:scrollY={scroll} /> -->

<!-- <div style:position="fixed">
  {scroll}
</div> -->

<div class="flex flex-col gap-10">
  <Header />

  <div class="mt-40">
    <Main />

    <div class="flex flex-col items-center justify-center gap-4 px-4">
      <Services />
      <WhyChoose />
    </div>

    <GoogleAvaliations />

    <div class="flex flex-col items-center justify-center gap-4 px-4">
      <AboutTheClinic />
    </div>

    <ImageCarrosel />

    <div class="flex flex-col items-center justify-center gap-4 px-4">
      <FAQ />
    </div>

    <Footer />
  </div>
</div>
