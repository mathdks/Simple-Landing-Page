<template>
  <section>
    <hooper :settings="hooperSettings" style="height: 400px">
        <slide>
          <div class="h-full flex flex-col justify-center place-items-center p-10">
            <Quote />
            <span>
              <p class="text-lg italic tracking-wide leading-relaxed text-center">
                Meu projeto ficou do jeito que eu sempre quis e foi entregue super rápido. Indico para todos!
              </p>
            </span>
            <span>
              <p class="text-lg font-bold italic tracking-wide leading-relaxed text-center">
                Karoline Ribeiro
              </p>
              <p class="text-sm italic tracking-wide leading-relaxed text-center">
                AP-KR052 - Novembro de 2020
              </p>
            </span>
          </div>
        </slide>
        <slide>
          <div class="h-full flex flex-col justify-center place-items-center p-10">
            <Quote />
            <span>
              <p class="text-lg italic tracking-wide leading-relaxed text-center">
                Acho incrível a atenção que eles dão aos detalhes! Eles já cuidaram de dois apartamentos meus e nunca houve problemas.
              </p>
            </span>
            <span>
              <p class="text-lg font-bold italic tracking-wide leading-relaxed text-center">
                João Pedro Fontes
              </p>
              <p class="text-sm italic tracking-wide leading-relaxed text-center">
                AP-JP221 - Fevereiro de 2021
              </p>
            </span>
          </div>
        </slide>
        <slide>
          <div class="h-full flex flex-col justify-center place-items-center p-10">
            <Quote />
            <span>
              <p class="text-lg italic tracking-wide leading-relaxed text-center">
                Eu já tive muitos problemas em obras anteriores e demorei a confiar na Tharali. Mesmo assim, decidi arriscar. O resultado foi incrível e agora eu sou um cliente fiel!
              </p>
            </span>
            <span>
              <p class="text-lg font-bold italic tracking-wide leading-relaxed text-center">
                Carlos Evangelista Neto
              </p>
              <p class="text-sm italic tracking-wide leading-relaxed text-center">
                CS-CEN1093 - Maio de 2020
              </p>
            </span>
          </div>
        </slide>
        <hooper-navigation slot="hooper-addons"></hooper-navigation>
    </hooper>
  </section>
</template>

<script>
import { Hooper, Slide, Navigation as HooperNavigation } from 'hooper';
import 'hooper/dist/hooper.css';

export default {
  name: 'App',
  components: {
    Hooper,
    Slide,
    HooperNavigation
  },
  data() {
    return {
      hooperSettings: {
        itemsToShow: 1,
        centerMode: true,
        autoPlay: true,
        playSpeed: '3000',
        infiniteScroll: true,
        vertical: true
      }
    };
  }
};
</script>