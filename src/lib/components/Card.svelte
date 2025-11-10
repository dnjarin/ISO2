<script>
  export let title = '';
  export let subtitle = '';
</script>

<article class="card">
  {#if title}<h3>{title}</h3>{/if}
  {#if subtitle}<p class="lead">{subtitle}</p>{/if}
  <div><slot /></div>
</article>