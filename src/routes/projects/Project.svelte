<script>
  export let image;
  export let title;
  export let href;
</script>

<div class="rounded p-4 flex flex-col gap-4 items-start dark:bg-slate-800 bg-slate-200">
    <h4 class="text-2xl">
      <a href={href} class="underline dark:text-blue-200 text-blue-900">{title}</a>
    </h4>
    {#if image}
      <img alt={title} src={image} class="w-48" />
    {/if}
    <p>
      <slot></slot>
    </p>
</div>
