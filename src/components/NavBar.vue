<template>
  <header class="header">
    <router-link
      class="w-10 h-10 absolute lg:fixed m-6 select-none outline-none"
      focusable="false"
      to="/"
    >
      <span>Jan Friebe</span>
    </router-link>
    <nav class="nav">
      <div class="spacer" />
      <div class="right">
        <router-link to="/about">
          About
        </router-link>
        <router-link to="/bookmarks" title="Bookmarks">
          <ri-bookmark-line />
        </router-link>
        <a href="https://twitter.com/jan_friebe" rel="noopener" target="_blank" title="Twitter" class="hidden md:block">
          <feather-twitter />
        </a>
        <a href="https://github.com/friebe" rel="noopener" target="_blank" title="GitHub" class="hidden md:block">
          <uil-github-alt />
        </a>
      </div>
    </nav>
  </header>
</template>

<style scoped>
.header h1 {
  margin-bottom: 0;
}

.logo {
  position: absolute;
  top: 1.5rem;
  left: 1.5rem;
}

.nav {
  padding: 2rem;
  width: 100vw;
  display: grid;
  grid-template-columns: auto max-content;
  box-sizing: border-box;
}

.nav > * {
  margin: auto;
}

.nav img {
  margin-bottom: 0;
}

.nav a {
  cursor: pointer;
  text-decoration: none;
  color: inherit;
  transition: opacity 0.2s ease;
  opacity: 0.6;
  outline: none;
}

.nav a:hover {
  opacity: 1;
  text-decoration-color: inherit;
}

.nav .right {
  display: grid;
  grid-gap: 1.2rem;
  grid-auto-flow: column;
}

.nav .right > * {
  margin: auto;
}
</style>
