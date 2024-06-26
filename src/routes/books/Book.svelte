<script>
  export let coverUrl;
  export let title;
  export let href;
  export let year;
  export let publisher;
</script>

<div class="flex flex-col gap-4 bg-slate-200 rounded p-4">
  <a href={href}>
    <img 
      src={coverUrl} 
      alt={title}
    >
  </a>
  <a href={href}><h3 class="text-2xl text-slate-700">{title}</h3></a>
  <div>{publisher}, {year}</div>
</div>