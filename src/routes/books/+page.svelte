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
    amazonHref="https://www.amazon.com/Web-API-Cookbook-JavaScript-Applications/dp/1098150694"
  >
    JavaScript gives web developers great power to create rich interactive browser experiences, and much of that power is provided by the browser itself. Modern web APIs enable web-based applications to come to life like never before, supporting actions that once required browser plug-ins.
  </Book>

  <Book
    title="Modern CSS"
    coverUrl={modernCss}
    publisher="Apress"
    year="2020"
    href="https://link.springer.com/book/10.1007/978-1-4842-6294-8"
    amazonHref="https://www.amazon.com/Modern-CSS-Master-Concepts-Development/dp/148426293X"
  >
    Come on a tour of “modern” CSS in 2020. This example-driven book demonstrates the concepts by showing code examples, screenshots, and diagrams to help clearly communicate the information.
  </Book>

  <Book
    title="Using Gatsby and Netlify CMS"
    coverUrl={gatsby}
    publisher="Apress"
    year="2020"
    href="https://link.springer.com/book/10.1007/978-1-4842-6297-9"
    amazonHref="https://www.amazon.com/Using-Gatsby-Netlify-CMS-JAMstack/dp/1484262964"
  >
    Leverage the powerful new combination of Gatsby and Netlify CMS, a free open source content management solution, to build blazing fast apps. This book shows you how to create a React-powered website using the Gatsby framework for the frontend, and Netlify CMS as the content backend. 
  </Book>
</div>