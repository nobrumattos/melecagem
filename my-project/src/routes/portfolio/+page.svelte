<script>
  let name = '';
  let email = '';
  let inquiry = '';

  function handleSubmit() {
      alert(`Obrigado, ${name}! Sua consulta foi enviada. Entraremos em contato em breve.`);
  }
</script>

<section class="bg-gray-700 p-8 rounded-lg shadow-lg max-w-6xl mx-auto mt-10">
  <header class="mb-6 text-center">
      <h1 class="text-4xl font-extrabold text-white mb-2">Portfólio de Melecagem</h1>
      <p class="text-gray-300 text-lg">Explore as obras vibrantes e criativas de Melissa Trugillo.</p>
  </header>

 <!-- Seção de Trabalhos Destacados -->
<section class="mb-8">
    <h2 class="text-3xl font-bold text-teal-400 mb-4">Trabalhos Destacados</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
        <!-- Exemplo de um trabalho -->
        <div class="bg-gray-800 rounded-lg overflow-hidden shadow-md">
            <img src="/obrona.jpg" alt="Trabalho 1" class="w-full h-64 object-cover">
            <div class="p-4">
                <h3 class="text-2xl text-white font-bold">Título da Obra 1</h3>
                <p class="text-gray-400 mt-2">Descrição breve da obra, técnica utilizada, e inspiração.</p>
            </div>
        </div>
        <!-- Repita o bloco abaixo para mais obras -->
        <div class="bg-gray-800 rounded-lg overflow-hidden shadow-md">
            <img src="/obrona2.jpg" alt="Trabalho 2" class="w-full h-64 object-cover">
            <div class="p-4">
                <h3 class="text-2xl text-white font-bold">Título da Obra 2</h3>
                <p class="text-gray-400 mt-2">Descrição breve da obra, técnica utilizada, e inspiração.</p>
            </div>
        </div>
        <div class="bg-gray-800 rounded-lg overflow-hidden shadow-md">
            <img src="/obrona3.jpg" alt="Trabalho 3" class="w-full h-64 object-cover">
            <div class="p-4">
                <h3 class="text-2xl text-white font-bold">Título da Obra 3</h3>
                <p class="text-gray-400 mt-2">Descrição breve da obra, técnica utilizada, e inspiração.</p>
            </div>
        </div>
        <div class="bg-gray-800 rounded-lg overflow-hidden shadow-md">
            <img src="/obrona4.jpg" alt="Trabalho 4" class="w-full h-64 object-cover">
            <div class="p-4">
                <h3 class="text-2xl text-white font-bold">Título da Obra 4</h3>
                <p class="text-gray-400 mt-2">Descrição breve da obra, técnica utilizada, e inspiração.</p>
            </div>
        </div>
    </div>
</section>


  <!-- Seção de Categorias de Arte -->
  <section class="mb-8">
      <h2 class="text-3xl font-bold text-teal-400 mb-4">Categorias de Arte</h2>
      <div class="flex flex-wrap justify-center space-x-4">
        <a href="/portfolio/desenhos" class="bg-gray-900 text-white p-4 rounded-lg shadow hover:bg-teal-500 transition">Desenhos</a>
        <a href="/portfolio/ilustraçoes" class="bg-gray-900 text-white p-4 rounded-lg shadow hover:bg-teal-500 transition">Ilustrações</a>
        <a href="/portfolio/digitalart" class="bg-gray-900 text-white p-4 rounded-lg shadow hover:bg-teal-500 transition">Esculturas</a>
          <!-- Adicione mais categorias conforme necessário -->
      </div>
  </section>

  <!-- Formulário para Consulta -->
  <section class="bg-gray-800 p-6 rounded-lg shadow-md">
      <header class="mb-4 text-center">
          <h2 class="text-3xl font-bold text-teal-400">Solicitar Mais Informações</h2>
          <p class="text-gray-300">Interessado em uma obra específica? Preencha o formulário abaixo.</p>
      </header>

      <form on:submit|preventDefault={handleSubmit} class="space-y-4">
          <div>
              <label class="block text-gray-400 mb-2" for="name">Nome</label>
              <input id="name" bind:value={name} class="w-full p-3 rounded bg-gray-900 text-white" type="text" placeholder="Seu Nome" required>
          </div>
          <div>
              <label class="block text-gray-400 mb-2" for="email">Email</label>
              <input id="email" bind:value={email} class="w-full p-3 rounded bg-gray-900 text-white" type="email" placeholder="seuemail@exemplo.com" required>
          </div>
          <div>
              <label class="block text-gray-400 mb-2" for="inquiry">Consulta</label>
              <textarea id="inquiry" bind:value={inquiry} class="w-full p-3 rounded bg-gray-900 text-white" rows="4" placeholder="Sua consulta sobre a obra" required></textarea>
          </div>
          <button class="bg-teal-500 hover:bg-teal-400 text-white font-bold py-2 px-4 rounded" type="submit">Enviar</button>
      </form>
  </section>
</section>
