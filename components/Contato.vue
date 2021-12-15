<template>
  <section>
    <form method="POST" action="https://simple-form.com/contato@tharali.com.br">
      <div class="justify-center text-center flex flex-col w-full">
        <label for="name" class="font-semibold text-lg">Nome</label>
        <input required type="text" id="name" name="Nome" placeholder="Seu nome completo" class="p-1 text-center w-full rounded-full border focus:outline-none focus:ring-2 focus:bg-blue-100">
        <label for="email" class="font-semibold text-lg">Email</label>
        <input required type="email" id="email" name="Email" placeholder="Seu e-mail" class="p-1 text-center w-full rounded-full border focus:outline-none focus:ring-2 focus:bg-blue-100">
        <label for="phone" class="font-semibold text-lg">Telefone</label>
        <input required type="phone" pattern="[0-9]{11}" id="phone" name="Telefone" placeholder="Seu telefone com DDD. Apenas números." class="p-1 text-center w-full rounded-full border focus:outline-none focus:ring-2 focus:bg-blue-100">
        <label class="font-semibold text-lg">O seu imóvel é:</label>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-col justify-between">
            <div><input type="radio" id="ap" value="Apartamento" name="Imóvel"><label for="ap"> Apartamento</label></div>
            <div><input type="radio" id="house" value="Casa" name="Imóvel"><label for="house"> Casa</label></div>
          </div>
        </div>
        <label class="font-semibold text-lg">Detalhes do imóvel:</label>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-row justify-between">
            <div><label for="size" class="font-semibold text-lg">Tamanho: </label></div>
            <div><input type="number" id="size" name="Tamanho" min="0" max="10000" placeholder="Ex: 150" class="p-1 text-center border-b-2 focus:outline-none focus:bg-blue-100"><label for="size" class="font-semibold"> m²</label></div>
          </div>
        </div>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-row justify-between">
            <div><label for="bath" class="font-semibold text-lg">Banheiros: </label></div>
            <div><input type="number" id="bath" name="Banheiros" min="0" max="10" placeholder="Ex: 3" class="p-1 text-center border-b-2 focus:outline-none focus:bg-blue-100"></div>
          </div>
        </div>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-row justify-between">
            <div><label for="bedroom" class="font-semibold text-lg">Dormitórios: </label></div>
            <div><input type="number" id="bedroom" name="Dormitórios" min="0" max="10" placeholder="Ex: 5" class="p-1 text-center border-b-2 focus:outline-none focus:bg-blue-100"></div>
          </div>
        </div>
        <label class="font-semibold text-lg">Serviço desejado:</label>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-col justify-between">
            <div><input type="checkbox" id="place1" value="Administração de Obras" name="Serviço1"> <label for="place1"> Administração de obra</label></div>
            <div><input type="checkbox" id="place2" value="Projeto" name="Serviço2"><label for="place2"> Projeto</label></div>
          </div>
        </div>
        <label for="detServ" class="font-semibold text-lg">Detalhes do serviço:</label>
        <textarea name="DetalhesDoServiço" id="detServ" cols="15" rows="6" placeholder="Descrição curta do serviço desejado. Ex: Projeto e administração de obra do banheiro da suíte e do lavabo." class="p-1 text-center w-full rounded-3xl border focus:outline-none focus:ring-2 focus:bg-blue-100"></textarea>
        <label class="font-semibold text-lg">Aceito receber uma resposta via:</label>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-col justify-between">
            <div><input type="checkbox" id="viaEmail" value="email" name="Resposta1"> <label for="viaEmail">E-mail</label></div>
            <div><input type="checkbox" id="viaWhatsapp" value="whatsapp" name="Resposta2"> <label for="viaWhatsapp">WhatsApp</label></div>
          </div>
        </div>
        <div class="place-items-center place-content-center flex">
          <div class="flex flex-row justify-between p-2">
            <input type="submit" value="Enviar" class="rounded-full bg-green-500 w-40 p-2 font-semibold text-lg text-white cursor-pointer"/>
          </div>
        </div>
      </div>
    </form>
  </section>
</template>

<script>
  export default {
  }
</script>