<script>
  import PageTitle from '$lib/components/PageTitle.svelte';

  export let data;
</script>

<svelte:head>
  <title>Articles | Joe Attardi</title>
</svelte:head>

<PageTitle subtitle="Articles by Joe Attardi">Articles</PageTitle>

<h3 class="text-3xl">LogRocket Articles</h3>

<section class="flex flex-col gap-4 mt-4">
  {#each data.logrocket as item}
    <article class="border border-slate-300 dark:border-slate-800 p-4 rounded">
      <h4 class="text-xl"><a href={item.href} class="text-blue-600 dark:text-blue-300">{item.title}</a></h4>
      <p>{item.summary}</p>
    </article>
  {/each}
</section>

<h3 class="mt-4 text-2xl">freeCodeCamp Articles</h3>

<section class="flex flex-col gap-4 mt-4">
  {#each data.freecodecamp as item}
    <article class="border border-slate-300 dark:border-slate-800 p-4 rounded">
      <h4 class="text-xl"><a href={item.href} class="text-blue-600 dark:text-blue-300">{item.title}</a></h4>
      <p>{item.summary}</p>
    </article>
  {/each}
</section>