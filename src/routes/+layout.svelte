<script>
    import NavBar from '../components/NavBar.svelte';
    import Footer from '../components/Footer.svelte';
  </script>
  
  <header>
    <NavBar />
  </header>
  
  <main>
    <slot />  <!-- This is where child pages will be rendered -->
  </main>
  
  <footer>
    <Footer />
  </footer>
  
  <style>
    header {
      background: #333;
      padding: 1rem;
      color: white;
    }
  
    main {
      padding: 20px;
      min-height: 80vh;
    }
  
    footer {
      margin-top: 20px;
    }
  </style>
  