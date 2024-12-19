<template>
  <div id="app">
    <header>
      <nav>
        <p class="h">Header</p>
        <router-link to="/page1" class="nav-link">Page 1</router-link>
        <router-link to="/page2" class="nav-link">Page 2</router-link>
        <router-link to="/page3" class="nav-link">Page 3</router-link>
      </nav>
    </header>

    <div class="layout">
      <aside class="menu">
        <ul>
          <a href="">Menu</a>
          <a href="">Section1</a>
          <a href="">Section2</a>
          <a href="">Section3</a>
          <a href="">Section4</a>
        </ul>
      </aside>

      <main>
        <router-view />
      </main>
    </div>

    <footer>
      Footer
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  background-color: #f4f4f4;
  padding: 10px;
  text-align: center;
}

header nav {
  display: flex;
  justify-content: center;
  gap: 20px;
  width: 1000px;
  justify-content: space-between;
}

header .nav-link {
  text-decoration: none;
  color: black;
}

header .nav-link.router-link-active {
  color: red;
  font-weight: bold;
}

.layout {
  display: flex;
  flex: 1;
  flex-direction: row;

}

.menu {
  width: 200px;
  background-color: #f8f8f8;
  padding: 20px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
  display: flex;
  flex: 1;
}

.menu ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
}

.menu a {
  margin: 10px 0;
}

main {
  flex: 1;
  padding: 20px;
  text-align: center;
}

footer {
  background-color: #f4f4f4;
  text-align: center;
  padding: 10px;
}
</style>
