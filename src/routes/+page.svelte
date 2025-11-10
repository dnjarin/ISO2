<script>
  import Card from '$lib/components/Card.svelte';
  import Button from '$lib/components/Button.svelte';
</script>

<h1>Inicio</h1>

<Card title="Bienvenido" subtitle="Ejemplo de evaluación SvelteKit">
  <p>Esta app demuestra: 3 componentes reutilizables, rutas y ruta dinámica.</p>
  <Button on:click={() => alert('Hola desde Home')}>Saludar</Button>
</Card>

<section style="margin-top:1rem;">
  <h2>Posts de ejemplo</h2>
  <ul>
    <li><a href="/posts/introduccion">Introducción</a></li>
    <li><a href="/posts/segundo-post">Segundo post</a></li>
  </ul>
</section>