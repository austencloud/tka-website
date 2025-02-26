/* Main Svelte Application File */
<script>
  import { onMount } from 'svelte';
  import Home from './components/Home.svelte';
  import About from './components/About.svelte';
  import Contact from './components/Contact.svelte';
  import NavBar from './components/NavBar.svelte';
  import { Router, Route } from 'svelte-routing';
</script>

<main>
  <NavBar />
  <Router>
    <Route path="/" component={Home} />
    <Route path="/about" component={About} />
    <Route path="/contact" component={Contact} />
  </Router>
</main>

<style>
  main {
    font-family: Arial, sans-serif;
    text-align: center;
    padding: 20px;
  }
</style>
