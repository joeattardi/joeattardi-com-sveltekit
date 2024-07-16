<script>
  export let subtitle;
</script>

<div class="mb-8">
  <h2 class="text-4xl font-bold text-sky-500"><slot></slot></h2>
  {#if subtitle}
    {subtitle}
  {/if}
</div>