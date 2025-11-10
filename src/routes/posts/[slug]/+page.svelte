<script>
  import { page } from '$app/stores';
  import Card from '$lib/components/Card.svelte';

  // Datos de ejemplo en memoria
  const posts = {
    'introduccion': {
      title: 'Introducción',
      body: 'Este es el primer post. Contenido dinámico basado en slug.'
    },
    'segundo-post': {
      title: 'Segundo Post',
      body: 'Contenido del segundo post.'
    }
  };

  // obtener slug desde la store page
  $: slug = $page.params.slug;
  $: post = posts[slug];
</script>

{#if post}
  <Card title={post.title}>
    <p>{post.body}</p>
  </Card>
{:else}
  <Card title="No encontrado">
    <p>El post "{slug}" no existe. Intenta: <a href="/">volver</a></p>
  </Card>
{/if}