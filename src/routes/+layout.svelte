<script>
  import '../app.css';
  import Navbar from '$lib/components/Navbar.svelte';
</script>

<div class="container">
  <Navbar />
  <main style="margin-top:1rem;"><slot /></main>
</div>