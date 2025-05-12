<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div>
      <a href="#" class="title_name">&lt;CHANG TINGWEI&gt;</a>
    </div>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <router-link to="/implementation">Implementation</router-link>
      <RouterLink to="/resumes">Resumes</RouterLink>
    </nav>
  </header>
  <main>
    <RouterView />
  </main>
  <footer>
    <div class="footer">&copy; copyright 2025 by Kitou</div>
  </footer>
</template>

<style lang="scss" scoped>
header {
  width: 1100px;
  // max-width: 1024px;
  box-sizing: border-box;
  padding: 16px;
  margin-bottom: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: sticky;
  top: 0px;
  z-index: 10;
  background-color: #fefff5;
  .title_name {
    font-size: 30px;
    font-weight: bold;
  }
  nav {
    a {
      display: inline-block;
      margin: 0 24px;
      font-size: 24px;

      &:hover {
        color: #e3c451;
      }
    }
  }
}
main {
  width: 100%;
  padding: 0 16px;
}
.footer {
  color: rgb(0, 0, 0, 0.7);
  font-size: 17px;
  background-color: #fefff5;
  text-align: center;
  padding: 10px 0;
  padding-bottom: 20px;
}
</style>
