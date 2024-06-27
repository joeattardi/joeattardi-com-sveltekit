<script>
    import { afterNavigate } from '$app/navigation';
    import List from 'phosphor-svelte/lib/List';
    import X from 'phosphor-svelte/lib/X';
    import NavLink from './NavLink.svelte';

    let expanded = false;

    function toggleNav() {
      expanded = !expanded;
    }

    afterNavigate(() => {
      expanded = false;
    });
</script>

<nav>
  <ul 
    class="p-4 flex flex-col justify-center fixed top-0 w-full left-0 h-full bg-blue-300 gap-4 md:flex-row md:relative md:bg-transparent md:flex md:items-center md:translate-x-0"
    class:translate-x-0={expanded}
    class:translate-x-full={!expanded}
  >
    <NavLink href="/books">Books</NavLink>
    <!-- <NavLink href="/projects">Projects</NavLink> -->
    <!-- <NavLink href="/articles">Articles</NavLink> -->
    <NavLink href="https://joeattardi.dev">Blog</NavLink>
  </ul>
</nav>

<button 
  type="button" 
  class="md:hidden z-10" 
  on:click={toggleNav}
  >
    {#if expanded}
      <X size={32} />
    {:else}
      <List size={32} />
    {/if}
</button>