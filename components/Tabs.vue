<template>
  <div class="flex flex-wrap px-5 md:px-0">
    <div class="w-full md:h-64 h-auto">
      <ul class="flex mb-0 list-none flex-wrap pt-3 pb-4 flex-row">
        <li class="flex-auto text-center">
          <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block" @click="toggleTabs(1)" :class="{'text-yellow-600 bg-white': openTab !== 1, 'text-white bg-yellow-600': openTab === 1}">
            Atendimento Personalizado
          </a>
        </li>
        <li class="flex-auto text-center">
          <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block" @click="toggleTabs(2)" :class="{'text-yellow-600 bg-white': openTab !== 2, 'text-white bg-yellow-600': openTab === 2}">
            Do seu jeito
          </a>
        </li>
        <li class="flex-auto text-center">
          <a class="text-xs font-bold uppercase px-5 py-3 shadow-lg rounded block" @click="toggleTabs(3)" :class="{'text-yellow-600 bg-white': openTab !== 3, 'text-white bg-yellow-600': openTab === 3}">
            Para qualquer lugar
          </a>
        </li>
      </ul>
      <div class="relative flex text-justify bg-white w-full mb-6 shadow-lg rounded">
        <div class="px-4 py-5 flex">
          <div class="md:w-96 w-auto">
            <div :class="{'hidden': openTab !== 1, 'block': openTab === 1}">
              <p>
                O nosso atendimento está pronto para te atender da forma mais atenciosa, prática e efetiva.
                <br />
                <br />
                Seja por <strong>ligação, e-mail ou WhatsApp, iremos atender todas as suas solicitações da forma que for mais fácil para você</strong>.
              </p>
            </div>
            <div :class="{'hidden': openTab !== 2, 'block': openTab === 2}">
              <p>
                Um lugar para chamar de casa é o sonho de todo mundo. E nós <strong>estamos aqui para ajudar na realização do seu sonho.</strong>
                <br />
                <br />
                Dessa forma, tudo será feito conforme o seu desejo.<br />
                <strong>Nós não faremos nenhum tipo de pressão para que você tome qualquer decisão.</strong>
              </p>
            </div>
            <div :class="{'hidden': openTab !== 3, 'block': openTab === 3}">
              <p>
                No mundo moderno as barreiras físicas estão cada vez menores.
                <br />
                <br />
                Então, <strong>se você mora em qualquer lugar do Brasil, a Tharali irá te atender</strong>.<br />
                Se você quer um projeto Tharali, nós estaremos disponíveis para te atender.
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
  name: "amber-tabs",
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
