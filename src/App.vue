<template>
  <div id="app">
    <header>
      <nav>
        <ul>
          <li><router-link to="/">Weather</router-link></li>
          <li><router-link to="/location">Location</router-link></li>
          <li><router-link to="/stopwatch">Stopwatch</router-link></li>
          <li><router-link to="/tictactoe">Tic Tac Toe</router-link></li>
          <li><router-link to="/photo">Photo</router-link></li>
        </ul>
      </nav>
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  text-align: center;
}

header {
  background: #56fff9;
  border-radius: 10px;
  padding: 12px;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

nav li {
  background-color: #ffb35d;
  display: inline-block;
  margin-right: 10px;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-weight: bold;
  padding: 10px;
  border-radius: 10px;
  
}

nav a {
  color: #fff;
  text-decoration: none;
}

nav li:hover {
  background-color: #4caf50;
  padding: 10px;
}
</style>
