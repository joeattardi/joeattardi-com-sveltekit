<script>
  export let href;
</script>

<li class="flex hover:bg-blue-200 rounded px-2 py-4 md:py-1">
  <a class="flex-grow text-center text-4xl md:text-lg" href={href}><slot></slot></a>
</li>
