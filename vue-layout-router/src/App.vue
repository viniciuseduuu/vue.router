<template>
  <div id="layout">
    <header>
      <h1>my projects</h1>
    </header>
    <aside>
      <nav>
        <router-link to="/" exact>Home</router-link>
        <router-link to="/products">Produtos</router-link>
        <router-link to="/contact">Contato</router-link>
        <router-link to="/about">Sobre nós</router-link>
      </nav>
    </aside>
    <main>
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
  #layout {
    font-family: Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;

    min-height: 100vh;
    width: 100vw;
    display: grid;
    grid-template-columns: 1fr 11fr;
    grid-template-rows: auto 1fr;

    grid-template-areas:
      'sidebar header'
      'sidebar main';
  }

  header {
    grid-area: header;
    height: 10vh;

    grid-area: sidebar;
  }

  aside nav {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    padding: 1rem;
  }

  main {
    grid-area: main;
  }
</style>


