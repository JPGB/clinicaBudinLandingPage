<script lang="ts">
  let width: number;
</script>

<!-- style:background-image="url(https://picsum.photos/{width}/320)" -->
<main
  bind:clientWidth={width}
  class="w-full h-80 text-[#f1f1f1] flex justify-center items-center bg-black/50"
>
  <div class="w-4/5 flex flex-col justify-center items-center gap-4">
    <p class="">Clinica Budin</p>
    <p class="">Especialistas em Implantes e prótese Dentária em Suzano</p>
    <p class="">Chega de esconder o sorriso ou sofrer para mastigar.</p>
    <button class="bg-amber-500 py-2 px-4 rounded-full text-[.7rem]">
      QUERO AGENDAR MINHA AVALIAÇÃO!
    </button>
    <div class="flex gap-4">
      <div
        class="w-8 h-8 bg-stone-300 border border-solid border-black rounded-full"
      ></div>
      <div
        class="w-8 h-8 bg-stone-300 border border-solid border-black rounded-full"
      ></div>
    </div>
    <p class="">+1000 pacientes atendidos</p>
  </div>
</main>
