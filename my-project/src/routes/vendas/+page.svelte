<script>
  export let title = 'Vendas';
</script>

<section class="bg-gray-900 py-16">
<div class="container mx-auto px-4">
  <header class="text-center mb-12">
    <h2 class="text-4xl font-extrabold text-white mb-4">{title}</h2>
    <p class="text-gray-300 text-lg">
      Explore e adquira as obras exclusivas de Melecagem. Cada peça é única e feita com atenção aos detalhes. Navegue pela nossa galeria de vendas para encontrar a arte perfeita para você.
    </p>
  </header>

  <!-- Grid de Amostras de Vendas -->
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
    <!-- Card de Exemplo -->
    <div class="bg-gray-800 p-6 rounded-lg shadow-lg transition-transform transform hover:scale-105">
      <img src="/obrona2.jpg" alt="Arte 1" class="w-full h-48 object-cover rounded-lg mb-4">
      <h3 class="text-xl font-semibold text-white mb-2">Desenho Digital 1</h3>
      <p class="text-gray-400 mb-2">Um exemplo de arte digital com influências do cartoon e hip-hop.</p>
      <p class="text-teal-400 font-bold mb-4">R$150,00</p>
      <button class="w-full bg-teal-600 text-white py-2 px-4 rounded-lg shadow-md hover:bg-teal-700 transition-colors duration-300">
        Adicionar ao Carrinho
      </button>
    </div>

    <!-- Card de Exemplo -->
    <div class="bg-gray-800 p-6 rounded-lg shadow-lg transition-transform transform hover:scale-105">
      <img src="/obrona3.jpg" alt="Arte 2" class="w-full h-48 object-cover rounded-lg mb-4">
      <h3 class="text-xl font-semibold text-white mb-2">Adesivo 1</h3>
      <p class="text-gray-400 mb-2">Adesivo com estilo único e vibrante, perfeito para personalizar seu espaço.</p>
      <p class="text-teal-400 font-bold mb-4">R$30,00</p>
      <button class="w-full bg-teal-600 text-white py-2 px-4 rounded-lg shadow-md hover:bg-teal-700 transition-colors duration-300">
        Adicionar ao Carrinho
      </button>
    </div>

    <!-- Card de Exemplo -->
    <div class="bg-gray-800 p-6 rounded-lg shadow-lg transition-transform transform hover:scale-105">
      <img src="/obrona4.jpg" alt="Arte 3" class="w-full h-48 object-cover rounded-lg mb-4">
      <h3 class="text-xl font-semibold text-white mb-2">Desenho Original</h3>
      <p class="text-gray-400 mb-2">Desenho feito à mão, capturando a essência do estilo Melecagem.</p>
      <p class="text-teal-400 font-bold mb-4">R$250,00</p>
      <button class="w-full bg-teal-600 text-white py-2 px-4 rounded-lg shadow-md hover:bg-teal-700 transition-colors duration-300">
        Adicionar ao Carrinho
      </button>
    </div>

    <!-- Card de Exemplo -->
    <div class="bg-gray-800 p-6 rounded-lg shadow-lg transition-transform transform hover:scale-105">
      <img src="/obrona.jpg" alt="Arte 4" class="w-full h-48 object-cover rounded-lg mb-4">
      <h3 class="text-xl font-semibold text-white mb-2">Ícone Exclusivo</h3>
      <p class="text-gray-400 mb-2">Ícone digital inspirado pelo estilo vibrante de Melecagem.</p>
      <p class="text-teal-400 font-bold mb-4">R$100,00</p>
      <button class="w-full bg-teal-600 text-white py-2 px-4 rounded-lg shadow-md hover:bg-teal-700 transition-colors duration-300">
        Adicionar ao Carrinho
      </button>
    </div>

    <!-- Mais cards podem ser adicionados aqui -->
  </div>

  <footer class="text-center mt-12">
    <p class="text-gray-300">
      !! ADICIONAR API DO PAYPAL PARA PAGAMENTOS PIX, CARTÃO OU BOLETO NA <a href="/vendas" class="text-teal-500 hover:underline">Vendas</a>. Agradecemos o seu interesse em apoiar o trabalho de Melecagem!
    </p>
  </footer>
</div>
</section>
