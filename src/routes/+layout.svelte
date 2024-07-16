<script>
  import '../app.css';
  import Header from './Header.svelte';
</script>

<div class="flex flex-col h-full">
  <Header />

  <div class="bg-slate-50 dark:bg-neutral-950 flex-grow">
    <main class="max-w-screen-lg m-auto p-4 text-black dark:text-neutral-200">
      <slot></slot>
    </main>
  </div>
</div>