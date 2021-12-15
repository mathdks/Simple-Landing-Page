<template>
  <div class="flex flex-wrap">
    <div class="w-full flex flex-col md:flex-row px-5 md:px-0">
      <div class="flex flex-col md:h-64 h-auto">
        <ul class="mb-0 list-none flex-wrap pt-3 pb-4 h-full">
          <li class="flex-auto text-center">
            <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block" @click="toggleTabs(1)" :class="{'text-yellow-600 bg-white': openTab !== 1, 'text-white bg-yellow-600': openTab === 1}">
              Administração de Obras
            </a>
          </li>
          <li class="flex-auto text-center">
            <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block" @click="toggleTabs(2)" :class="{'text-yellow-600 bg-white': openTab !== 2, 'text-white bg-yellow-600': openTab === 2}">
              Projeto
            </a>
          </li>
        </ul>
      </div>
      <div class="relative flex text-justify bg-white w-full mb-6 shadow-lg rounded">
        <div class="px-4 py-5 flex">
          <div class="md:w-96 w-auto">
            <div :class="{'hidden': openTab !== 1, 'block': openTab === 1}">
              <p>
                Tenha a <strong>certeza e tranquilidade</strong> de que a sua obra será executada da maneira correta.
                <br />
                <br />
                Afinal, <strong>você não precisa ter dor de cabeça durante a sua obra.</strong>
                <br />
                Deixe que a Tharali tome conta de tudo para que você possa focar suas energias em outros assuntos.
              </p>
            </div>
            <div :class="{'hidden': openTab !== 2, 'block': openTab === 2}">
              <p class="text-justify">
                A sua casa precisa ter a sua cara.
                <br />
                <br />
                E se você deseja uma casa <strong>linda, moderna e aconchegante</strong>, a Tharali é ideal para você.
                <br />
                A nossa equipe criativa criará um projeto perfeito, com tudo o que você precisa para aproveitar todo o <strong>conforto, segurança e felicidade</strong> na sua casa.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      openTab: 1
    }
  },
  methods: {
    toggleTabs: function(tabNumber){
      this.openTab = tabNumber
    }
  }
}
</script>
