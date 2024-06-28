<script>
  import PageTitle from '$lib/components/PageTitle.svelte';

  export let data;

  console.log(data);
</script>

<PageTitle>Articles</PageTitle>

<h3 class="text-3xl">LogRocket Articles</h3>

<section class="flex flex-col gap-4 mt-4">
  {#each data.logrocket as item}
    <article>
      <h4 class="text-xl"><a href={item.href} class="text-blue-600">{item.title}</a></h4>
      <p>{item.summary}</p>
    </article>
  {/each}
</section>

<h3 class="mt-4 text-2xl">freeCodeCamp Articles</h3>

<section class="flex flex-col gap-4 mt-4">
  {#each data.freecodecamp as item}
    <article>
      <h4 class="text-xl"><a href={item.href} class="text-blue-600">{item.title}</a></h4>
      <p>{item.summary}</p>
    </article>
  {/each}
</section>