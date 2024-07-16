<script>
  export let href;
</script>

<li class="flex hover:bg-blue-200 dark:hover:bg-blue-950 rounded px-2 py-4 md:py-1 text-black dark:text-sky-100">
  <a class="flex-grow text-center text-4xl md:text-lg" href={href}><slot></slot></a>
</li>
