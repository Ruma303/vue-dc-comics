<template>
  <header>
    <img
      src="@/img/dc-logo.png"
      alt=""
      class="header-logo"
    >
    <nav>
      <ul>
        <li
          v-for="eleMenu in arrMenu"
          :key="eleMenu.text"
        >
          <a :href="eleMenu.url">{{ eleMenu.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderSection',
  data() {
    return {
      arrMenu: [
        {
          url: '#Characters',
          text: 'Characters',
        },
        {
          url: '#Comics',
          text: 'Comics',
        },
        {
          url: '#Movies',
          text: 'Movies',
        },
        {
          url: '#TV',
          text: 'TV',
        },
        {
          url: '#Games',
          text: 'Games',
        },
        {
          url: '#Collectibles',
          text: 'Collectibles',
        },
        {
          url: '#Videos',
          text: 'Videos',
        },
        {
          url: '#Fans',
          text: 'Fans',
        },
        {
          url: '#News',
          text: 'News',
        },
        {
          url: '#Shop',
          text: 'Shop',
        },
      ],
    };
  },
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
nav li a:hover {
  color: rgb(0, 138, 255);
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
