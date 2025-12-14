<script lang="ts">
  const faq = [
    {
      question: "A harmonização facial muda muito o rosto?",
      response:
        "Na Clínica Budin, prezamos por resultados naturais. A harmonização é feita com muito critério, respeitando os traços de cada pessoa. O objetivo é valorizar sua beleza e trazer mais equilibrio ao resto, sem exageros.",
    },
    {
      question: "É possivel parcelar os procedimentos?",
      response:
        "Sim! Oferecemos diversas formas de pagamento, inclusive parcelamento no cartão. Na avaliação, explicamos todos os valores com transparência para você se programar com tranquilodade.",
    },
    {
      question: "Como fáco para agendar uma avaliação?",
      response:
        "É só clicar no botão de WhatsApp aqui na página e falar diretamente com nossa equipe. Vamos tirar suas dúvidas e agendar sue atendimento no melhor dia e horário para você!",
    },
    {
      question: "Quanto tempo dura o procedimento de prótese ou implante?",
      response:
        "O tempo pode variar de acordo com o caso. No geral, a colocação do implante dura cerca de 1 hora, e a recuperação é rápida. Já a confecção da prótese pode levar alguns dias, pois ela é feita sob medida para garantir conforto e estética.",
    },
  ];
</script>

<div class="flex flex-col items-center justify-center text-center">
  <h1 class="mt-2 text-2xl font-bold">Perguntas Frequentes</h1>
  {#each faq as faqItem}
    <div class="p-4 my-4 border-gray-300 rounded-lg">
      <h2 class="mb-2 font-semibold">{faqItem.question}</h2>
      <p>{faqItem.response}</p>
    </div>
  {/each}
</div>
