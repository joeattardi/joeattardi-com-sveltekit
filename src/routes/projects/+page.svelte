<script>
  import PageTitle from '$lib/components/PageTitle.svelte';
  import Project from './Project.svelte';
</script>

<svelte:head>
  <title>Projects | Joe Attardi</title>
</svelte:head>

<PageTitle>Projects</PageTitle>

<h3 class="text-3xl my-4">Open Source</h3>

<div class="grid grid-cols-2 gap-8">
  <Project
    title="json-colorizer"
    href="https://npmjs.com/package/json-colorizer"
  >
    An npm package to pretty-print JSON data with syntax highlighting.
  </Project>

  <Project
    title="promise-poller"
    href="https://www.npmjs.com/package/promise-poller"
  >
    An npm package that provides a Promise based interface for performing polling operations.
  </Project>
</div>

<h3 class="text-3xl my-4">Education and Training</h3>

<Project
  title="Build a Toast Notification System With Svelte (educative.io)"
  href="https://www.educative.io/projects/build-a-toast-notification-system-with-svelte"
>
  <p class="mb-4">A guided project series on building a basic toast notification system in a Svelte application. Published by <a href="https://educative.io">Educative</a>.</p>

  <p>
    In this project, we will start working on a skeleton Svelte application and incorporate a store to effectively manage notification information. After this, we will create Svelte components designed to subscribe to the store and facilitate the display of these notifications.
  </p>
</Project>
