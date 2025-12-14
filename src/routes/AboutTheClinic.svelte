<script lang="ts">
  const pics = ["", "", ""];
</script>

<div class="text-2xl flex flex-col justify-center items-center">
  <p class="">Sobre a</p>
  <p class="font-bold">Clínica Budin</p>
</div>

<p class="text-center w-4/5">
  Localizada no coração de Suzano, a Clínica Budin une tecnologia, empatia e
  excelência para oferecer o melhor da odotontologia e estética facil.
  <br />
  Seu sorriso e bem-estar são a nossa prioridade.
</p>

<div class="flex justify-center items-center flex-col gap-4 w-4/5">
  {#each pics as pic}
    <img src={pic} alt="" class="w-full h-40" />
  {/each}
</div>

<button class="rounded-full bg-amber-500 py-2 text-[#f1f1f1] px-2">
  Agendar minha avaliação gratuita agora!
</button>
