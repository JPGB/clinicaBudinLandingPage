<script lang="ts">
  import HealthiconsDoctor from "~icons/healthicons/doctor";
  import MapDentist from "~icons/map/dentist";

  const items = [
    { icon: HealthiconsDoctor, text: "Atendimento humanizado" },
    { icon: HealthiconsDoctor, text: "Implantes com carga imediata" },
    { icon: HealthiconsDoctor, text: "Harminização facial natural" },
    { icon: HealthiconsDoctor, text: "Qualidade dos materiais" },
    { icon: HealthiconsDoctor, text: "Localização central em Suzano" },
  ];
</script>

<div class=" flex flex-col justify-center items-center text-2xl">
  <p class="">Porque escolher a</p>
  <p class=""><b>Clínica Budin? </b></p>
</div>

<div class="flex flex-wrap justify-evenly gap-4 text-2xl p-4">
  {#each items as item}
    <div class="grow-0 shrink-0 basis-20">
      <div class="flex flex-col justify-center items-center">
        <item.icon class="text-5xl text-amber-500" />
        <div class="text-center text-xs">{item.text}</div>
      </div>
    </div>
  {/each}
</div>

<img src="" alt="dentista" class="bg-amber-200 w-4/5 h-40 rounded-xl" />

<button
  class="rounded-full bg-amber-500 py-2 text-[#f1f1f1] px-2 hover:bg-amber-950"
>
  Agendar minha avaliação gratuita agora!
</button>
