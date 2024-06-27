<script>
  export let coverUrl;
  export let title;
  export let href;
  export let year;
  export let publisher;
  export let amazonHref;
</script>

<div class="max-w-md flex flex-col gap-4 bg-slate-200 rounded p-4">
  <a href={href} class="overflow-hidden">
    <img
      class="transition-transform duration-500 hover:-rotate- hover:scale-105"
      src={coverUrl} 
      alt={title}
    >
  </a>
  <a href={href}><h3 class="text-2xl font-bold text-slate-700">{title}</h3></a>
  <div>{publisher}, {year}</div>
  <a class="bg-amber-500 px-2 py-1 flex items-center gap-2 rounded self-start text-center" href={amazonHref}>
    Get {title} on Amazon
  </a>
  <p><slot></slot></p>
</div>
