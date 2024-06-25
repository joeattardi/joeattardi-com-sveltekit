<script>
  import '../app.css';
  import Header from './Header.svelte';
</script>

<div class="flex flex-col h-full">
  <Header />

  <div class="bg-slate-50 flex-grow">
    <main class="max-w-screen-lg m-auto">
      <slot></slot>
    </main>
  </div>
</div>