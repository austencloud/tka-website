<script>
  import { onMount } from 'svelte';
  let links = [
    { name: 'Home', href: '/' },
    { name: 'About', href: '/about' },
    { name: 'Contact', href: '/contact' }
  ];
</script>

<nav class="navbar">
  {#each links as link}
    <a href={link.href}>{link.name}</a>
  {/each}
</nav>

<style>
  .navbar {
    display: flex;
    gap: 1rem;
    padding: 1rem;
    background: #333;
    color: white;
  }
  a {
    color: white;
    text-decoration: none;
  }
</style>



