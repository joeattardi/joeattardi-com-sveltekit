<script>
  import PageTitle from '$lib/components/PageTitle.svelte';
  import Book from './Book.svelte';

  import webApiCookbook from './web-api-cookbook-cover.png';
  import modernCss from './modern-css-cover.jpeg';
  import gatsby from './gatsby-cover.jpeg';
</script>

<svelte:head>
  <title>Books | Joe Attardi</title>
</svelte:head>

<PageTitle>Books</PageTitle>

<div class="flex gap-8 flex-wrap">
  <Book
    title="Web API Cookbook"
    coverUrl={webApiCookbook}
    publisher="O'Reilly Media"
    year="2024"
    href="https://learning.oreilly.com/library/view/web-api-cookbook/9781098150686/"
  />

  <Book
    title="Modern CSS"
    coverUrl={modernCss}
    publisher="Apress"
    year="2020"
    href="https://link.springer.com/book/10.1007/978-1-4842-6294-8"
  />

  <Book
    title="Using Gatsby and Netlify CMS"
    coverUrl={gatsby}
    publisher="Apress"
    year="2020"
    href="https://link.springer.com/book/10.1007/978-1-4842-6297-9"
  />
</div>