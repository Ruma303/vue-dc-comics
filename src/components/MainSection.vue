<template>
  <main>
    <div class="top-main" />
    <div class="bottom-main">
      <h1 id="current-series">
        CURRENT SERIES
      </h1>
      <CardPage
        v-for="i in arrData"
        :key="i.series"
        class="card"
        :thumb="i.thumb"
        :series="i.series"
      />
      <h1 id="load">
        LOAD MORE
      </h1>
    </div>
  </main>
</template>

<script>
import CardPage from "./CardPage.vue";

export default {
  name: "MainSection",
  components: {
    CardPage,
  },
  data() {
    return {
      arrData: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          series: "Action Comics",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          series: "American Vampire 1976",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          series: "Aquaman",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          series: "Batgirl",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          series: "Batman",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          series: "Batman Beyond",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          series: "Batman/Superman",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          series: "Batman/Superman Annual",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          series: "Batman: The Joker War Zone",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          series: "Batman: Three Jokers",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          series: "Batman: White Knight Presents: Harley Quinn",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          series: "Catwoman",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
main {
  margin: 0 auto;
}
#current-series {
  color: white;
  font-size: 1.4rem;
  padding: 0.5rem;
  background-color: rgb(15, 130, 247);
  white-space: nowrap;
  position: absolute;
  left: 2rem;
  top: 24.5rem;
  z-index: 3;
}
main .top-main{
  width: 100%;
  height: 300px;
  background-image: url("@/img/jumbotron.jpg");
  object-position: center;
}
main .bottom-main {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 1rem;
  width: 100%;
  height: 50rem;
  padding: 3rem 1rem;
  margin: 0 auto;
}
#load {
  color: white;
  font-size: 1rem;
  padding: 0.5rem;
  background-color: rgb(15, 130, 247);
  white-space: nowrap;
  position: absolute;
  left: 46.5vw;
  top: 72.5rem;
  z-index: 3;
  cursor: pointer;
}
</style>
