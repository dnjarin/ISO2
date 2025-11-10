<nav class="navbar container" role="navigation">
  <a class="nav-brand" href="/">Mi App</a>
  <div class="nav-links">
    <a href="/">Inicio</a>
    <a href="/pagina-fija">Página fija</a>
    <a href="/posts/introduccion">Ejemplo dinámico</a>
  </div>
  <div style="margin-left:auto">
    <slot name="actions"></slot>
  </div>
</nav>