<template>
  <nav class="custom-navbar">
    <a class="navbar-brand" href="#">MyWebsite</a>
    <a class="nav-link" href="#">Home</a>
    <a class="nav-link" href="#">About</a>
    <a class="nav-link" href="#">Contact</a>
    <div class="search-form">
      <input type="text" placeholder="Search" />
      <button type="submit">Search</button>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.custom-navbar {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: black;
  padding: 10px 50px;
}

.nav-link, .navbar-brand {
  color: white;
  transition: 0.3s;
  text-decoration: none;
}

.nav-link:hover {
  background-color: grey;
  color: black;
  padding: 5px 10px;
  border-radius: 5px;
}

.search-form {
  display: flex;
  align-items: center;
}

.search-form input {
  padding: 5px;
  border: none;
  border-radius: 5px 0 0 5px;
  outline: none;
}

.search-form button {
  padding: 5px 10px;
  border: none;
  background-color: white;
  color: black;
  cursor: pointer;
  border-radius: 0 5px 5px 0;
  transition: 0.3s;
}

.search-form button:hover {
  background-color: grey;
  color: white;
}
</style>
