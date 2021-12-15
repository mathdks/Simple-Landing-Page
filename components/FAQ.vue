<template>
  <section>
    <o-collapse class="card" animation="slide" v-for="(collapse, index) of collapses" :key="index" :open="isOpen == index" @open="isOpen = index">
      <div slot="trigger" slot-scope="props" class="card-header" role="button">
        <p class="card-header-title">
          {{ collapse.title }}
        </p>
        <a class="card-header-icon">
          <o-icon :icon="props.open ? 'caret-up' : 'caret-down'"> </o-icon>
        </a>
      </div>
      <div class="card-content">
        <div class="content text-justify">
          {{ collapse.text }}
        </div>
      </div>
    </o-collapse>
  </section>
</template>

<script>
  export default {
    data() {
      return {
        isOpen: 0,
        collapses: [
          {
            title: 'Quanto tempo demora para o meu projeto ficar pronto?',
            text: 'Essa pergunta não possui uma resposta exata. Tudo depende do nível de detalhes que o projeto necessita. A grande maioria dos projetos costumam ficar prontos em até 15 dias, mas existem casos que podem levar um tempo maior para tudo ficar pronto.'
          },
          {
            title: 'Se eu pedir um orçamento eu sou obrigado a fechar o negócio?',
            text: 'Não. Você não é obrigado a nada. O orçamento é enviado totalmente sem compromisso. Você não é obrigado a fechar o negócio.'
          },
          {
            title: 'Mudei de ideia sobre um detalhe do meu projeto, posso pedir para ser alterado?',
            text: 'Com certeza. O seu projeto precisa ficar do jeito que você sempre quis, e alterações serão necessárias para alcançar esse objetivo.'
          }
        ]
      }
    }
  }
</script>

<style>
  .card {
    background-color: #fff;
    box-shadow: 0 2px 3px hsla(0, 0%, 4%, 0.1), 0 0 0 1px hsla(0, 0%, 4%, 0.1);
    color: #4a4a4a;
    max-width: 100%;
    position: relative;
  }
  .card-header {
    background-color: transparent;
    align-items: stretch;
    box-shadow: 0 1px 2px hsla(0, 0%, 4%, 0.1);
    display: flex;
  }
  .card-header-title {
    align-items: center;
    color: #363636;
    display: flex;
    flex-grow: 1;
    font-weight: 700;
    padding: 0.75rem;
    margin: 0;
  }
  .card-header-icon {
    align-items: center;
    cursor: pointer;
    display: flex;
    padding: 0.75rem;
    justify-content: center;
  }
  .card-content {
    padding: 1.5rem;
    background-color: transparent;
  }
</style>