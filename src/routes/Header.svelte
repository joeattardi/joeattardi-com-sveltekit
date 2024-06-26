<script>
    import Nav from './Nav.svelte';
</script>

<header class="p-4 bg-sky-100">
  <div class="flex items-center max-w-screen-lg m-auto justify-between">
    <h1 class="text-2xl">
      <a href="/" class="flex items-center gap-2 font-bold">
        <img src="/site-logo.png" alt="Laptop icon" class="w-12">
        <span class="text-sky-500">Joe</span> <span class="text-blue-500">Attardi</span>
      </a>
    </h1>
    <Nav />
  </div>
</header>
