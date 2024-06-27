<script>
  export let icon;
  export let href;
  export let title;
</script>

<a
  href={href} 
  class="text-4xl  bg-indigo-700 p-2 text-white rounded-md hover:scale-105 transition-transform"
  title={title}
>
  <svelte:component this={icon} />
</a>