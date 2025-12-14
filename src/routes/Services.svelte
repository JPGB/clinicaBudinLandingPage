<script lang="ts">
  let width: number;

  const services = [
    {
      title: "Implantes Dentários",
      description:
        "Restaure seu sorriso com segurança e conforto. Implante com carga imediata disponivel.",
      bgImage: "https://picsum.photos/",
    },
    {
      title: "Próteses",
      description:
        "Estética e funcionalidade em um só lugar. Soluções sob medidda para você.",
      bgImage: "https://picsum.photos/",
    },
    {
      title: "Harmonização Facial",
      description:
        "Tratamentos modernos para valorizar sua beleza de forma natual e segura.",
      bgImage: "https://picsum.photos/",
    },
  ];
</script>

<div class="flex items-center justify-center flex-col text-center gap-4 py-8">
  <h2 class="text-3xl">Conheça nossos serviços</h2>
  <p class="">
    Diversos procedimentos para melhorar a qualidade de vida dos nosso
    pacientes.
  </p>
  <div
    class="flex items-center justify-center text-center gap-4 py-8 flex-wrap"
  >
    {#each services as service}
      <div
        style:background-image="url({service.bgImage})"
        class="bg-amber-600 p-8 flex justify-end items-center flex-col h-80 gap-4 rounded-2xl text-[#f1f1f1] w-72"
      >
        <h3 class="">{service.title}</h3>
        <p class="text-sm">{service.description}</p>
        <button
          class="border-white border border-solid py-2 px-4 rounded-full text-[.7rem]"
          >Agende sua avaliação!</button
        >
      </div>
    {/each}
  </div>
</div>
