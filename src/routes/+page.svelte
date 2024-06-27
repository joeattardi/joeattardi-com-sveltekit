<script>
  import LinkedinLogo from 'phosphor-svelte/lib/LinkedinLogo';
  import GithubLogo from 'phosphor-svelte/lib/GithubLogo';
  import Envelope from 'phosphor-svelte/lib/Envelope';
  import XLogo from 'phosphor-svelte/lib/XLogo';
  import ContactLink from '$lib/components/ContactLink.svelte';
</script>

<svelte:head>
  <title>Joe Attardi</title>
</svelte:head>

<div class="p-4 flex flex-col items-center md:items-start md:flex-row gap-4">
  <img 
    src="/undraw_programming_re_kg9v.svg" 
    alt="Joe Attardi"
    class="w-48 md:w-64"
  >
  <div class="flex flex-col gap-2">
    <h2 class="text-center text-4xl md:text-left md:text-6xl font-bold"><span class="text-sky-500">Joe</span> <span class="text-blue-500">Attardi</span></h2>
    <p class="text-center text-2xl md:text-left md:text-3xl">
      I'm a software developer and author from the Boston area with over 20 years of experience.
    </p>
    <div class="flex flex-row gap-4 m-auto md:m-0 md:mt-4 mt-4">
      <ContactLink title="Email" icon={Envelope} href="mailto:jattardi@gmail.com" />
      <ContactLink title="Twitter/X" icon={XLogo} href="https://twitter.com/JoeAttardi" />
      <ContactLink title="GitHub" icon={GithubLogo} href="https://github.com/joeattardi" />
      <ContactLink title="LinkedIn" icon={LinkedinLogo} href="https://linkedin.com/in/joeattardi" />
    </div>
  </div>
</div>

