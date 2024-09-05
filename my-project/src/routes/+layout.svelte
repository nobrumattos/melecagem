<script>
  import '../app.css';
</script>

<header class="relative z-20 bg-gradient-to-r from-purple-900 via-gray-900 to-purple-900 text-white py-4 border-b-2 border-cyber-blue shadow-lg">
  <div class="container mx-auto flex justify-between items-center px-4">
    <!-- Título Melecagem com estilo hip-hop cartoon sem efeito neon -->
    <h1 class="text-5xl font-extrabold font-hiphop">
      <a href="/" class="text-white hover:text-hiphop-pink">Melecagem</a>
    </h1>
    <nav>
      <ul class="flex space-x-6 text-cyber-cyan">
        <li><a href="/biografia" class="nav-link">Biografia</a></li>
        <li><a href="/portfolio" class="nav-link">Portfólio</a></li>
        <li><a href="/vendas" class="nav-link">Vendas</a></li>
      </ul>
    </nav>
  </div>
</header>

<main class="relative text-white min-h-screen py-8">
  <div class="container mx-auto px-4">
    <slot></slot> <!-- Onde o conteúdo das páginas será injetado -->
  </div>
</main>


<footer class="relative z-20 bg-gradient-to-r from-purple-900 via-gray-900 to-purple-900 text-white py-4 border-t-2 border-cyber-blue shadow-inner">
  <div class="container mx-auto text-center px-4">
    <p class="text-cyber-cyan">&copy; 2024 Meu Site. Todos os direitos reservados.</p>
  </div>
</footer>

<style>
  /* Fonte personalizada estilo hip-hop cartoon */
  @import url('https://fonts.googleapis.com/css2?family=Rubik+Wet+Paint&display=swap');

  /* Estilo hip-hop para o título sem efeito neon */
  .font-hiphop {
    font-family: 'Rubik Wet Paint', cursive;
    letter-spacing: 2px;
  }

  /* Efeito hover para mudar a cor do texto para rosa */
  .hover\:text-hiphop-pink:hover {
    color: #ff00ff;
    transition: color 0.3s ease;
  }

  /* Cores e transições para os links de navegação */
  .nav-link {
    position: relative;
    text-transform: uppercase;
    padding: 0.25rem 0.5rem;
    transition: color 0.3s ease;
  }

  .nav-link::before {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    bottom: -2px;
    left: 50%;
    transform: translateX(-50%);
    background-color: #ff00ff;
    visibility: hidden;
    transition: all 0.3s ease-in-out;
  }

  .nav-link:hover::before {
    visibility: visible;
    width: 100%;
  }

  .nav-link:hover {
    color: #ff00ff;
  }

  /* Estilos de cores para o tema cyberpunk */
  .text-cyber-cyan {
    color: #00ffff;
  }

  .text-cyber-pink {
    color: #ff00ff;
  }

  .bg-cyber-blue {
    background-color: #0f4c81;
  }
</style>
