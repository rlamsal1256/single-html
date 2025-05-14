<script>
  import Router from 'svelte-spa-router';
  import Home from './routes/Home.svelte';
  import About from './routes/About.svelte';

  const routes = {
      '/': Home,
      '/about': About
  };
</script>

<nav class="p-4 bg-gray-200 flex gap-4">
  <a href="#/">Home</a>
  <a href="#/about">About</a>
</nav>

<main class="p-4">
  <Router {routes} />
</main>
