<template>
  <header>
    <img src="@/img/dc-logo.png" alt="" class="header-logo">
    <nav>
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEOS</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderSection',
};
</script>

<style lang="scss" scoped>
header{
  background-color: white;
  height: 171px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 100%;
  padding: 1.5rem;
}
header a {
  color: black;
}
.header-logo{
  max-width: 4rem;
  max-height: 4rem;
}
nav ul {
  display: flex;
  justify-content: space-around;
  align-items: center;
  gap: 2rem;
  height: 100%;
}
</style>
