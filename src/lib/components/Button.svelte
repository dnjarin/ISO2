<script>
  export let variant = 'primary';
  export let onClick = () => {};
</script>

<button class="btn {variant === 'primary' ? 'btn-primary' : 'btn-outline'}" on:click={onClick}>
  <slot>Acción</slot>
</button>