<script>
  import SocialLinks from "./SocialLinks.svelte";

</script>

<nav class="navbar">
  <img src="/logo.png" alt="The Kinetic Alphabet" class="logo" />
  <div class="nav-links">
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/contact">Contact</a>
  </div>
  <SocialLinks />
</nav>

<style>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    background: #333;
    color: white;
  }
  .logo {
    height: 50px;
  }
</style>
