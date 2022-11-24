<template>
  <footer>
      <ul class="top-footer">
        <li>
          <img src="@/img/buy-comics-digital-comics.png" alt="" class="img-figure">
          <span class="img-text">digital comics</span>
        </li>
        <li>
          <img src="@/img/buy-comics-merchandise.png" alt="" class="img-figure">
          <span class="img-text">dc merchandise</span>
        </li>
        <li>
          <img src="@/img/buy-comics-subscriptions.png" alt="" class="img-figure">
          <span class="img-text">subscription</span>
        </li>
        <li>
          <img src="@/img/buy-comics-shop-locator.png" alt="" class="img-figure">
          <span class="img-text">comic shop locator</span>
        </li>
        <li>
          <img src="@/img/buy-dc-power-visa.svg" alt="" class="img-figure">
          <span class="img-text">dc power visa</span>
        </li>
      </ul>
    <div class="middle-footer">
      <div class="middle-footer-lt">
        <ul class="middle-footer-lt-ul">
          <li>
            <ul class="first-col">
              <li class="link-list">
                <h1>DC COMICS</h1>
                <span>Characters</span>
                <span>Comics</span>
                <span>Movies</span>
                <span>TV</span>
                <span>Games</span>
                <span>Videos</span>
                <span>News</span>
              </li>
              <li class="link-list">
                <h1>SHOP</h1>
                <span>Shop DC</span>
                <span>Shop DC Collectibles</span>
              </li>
            </ul>
          </li>
          <li class="link-list">
            <h1>DC</h1>
            <span>Terms Of Use</span>
            <span>Privacy policy (New)</span>
            <span>Ad Choise</span>
            <span>Advertising</span>
            <span>Jobs</span>
            <span>Subscription</span>
            <span>Talent Workspace</span>
            <span>CPSC Certificates</span>
            <span>Ratings</span>
            <span>Shop Help</span>
            <span>Contac Us</span>
          </li>
          <li class="link-list">
            <h1>SITES</h1>
            <span>DC</span>
            <span>MAD Magazine</span>
            <span>DC Kids</span>
            <span>DC Universe</span>
            <span>DC Power Visa</span>
          </li>
        </ul>
      </div>
      <div class="middle-footer-rt"><img src="@/img/dc-logo-bg.png" alt=""></div>
    </div>
    <div class="bottom-footer">
      <div class="bottom-footer-lt">
        <button class="btn-signup">SIGN-UP NOW!</button>
      </div>
      <div>
        <ul class="bottom-footer-rt">
          <li id="title-follow">FOLLOW US</li>
          <li><img src="@/img/footer-facebook.png" alt=""></li>
          <li><img src="@/img/footer-twitter.png" alt=""></li>
          <li><img src="@/img/footer-youtube.png" alt=""></li>
          <li><img src="@/img/footer-pinterest.png" alt=""></li>
          <li><img src="@/img/footer-periscope.png" alt=""></li>
        </ul>
      </div>
    </div>
    <div class="rest-footer"></div>
  </footer>
</template>

<script>
export default {
  name: 'FooterSection',
};
</script>

<style lang="scss" scoped>
//variabili scss
$color_blue:rgb(0, 138, 255);

.top-footer,
.bottom-footer,
.rest-footer{
  position: relative;
  z-index: 2;
}
.top-footer{
  background-color: $color_blue;
  height: 189px;//TODO: rendi dinamico
}
.middle-footer{
  background-image: url('@/img/footer-bg.jpg');
  height: 480px; //TODO: rendi dinamico
  background-repeat: none;
}
.bottom-footer{
  background-color: rgb(47, 47, 47);
  height: 157px;//TODO: rendi dinamico
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.rest-footer{
  background-color: rgb(32, 32, 32);
  height: 50vh;//TODO: rendi dinamico
}
.top-footer {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 5rem;
  width: 100%;
  white-space: nowrap;
}
.top-footer li {
  display: flex;
  align-items: center;
  gap: 1rem;
  color: white;
  text-transform: uppercase;
}
.top-footer img{
  max-width: 4rem;
  max-height: 4rem;
}
.middle-footer {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.middle-footer-lt-ul{
  display: flex;
  gap: 2rem;
}
.middle-footer h1{
  color: white;
  font-size: 1.5rem;
}
.middle-footer span{
  color: grey;
}
.first-col{
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
.link-list{
  display: flex;
  flex-direction: column;
  gap: .5rem;
}
.link-list h1{
  margin-bottom: 0.5rem;
}
.link-list span{
  cursor: pointer;
  font-size: .8rem;
}
.middle-footer-rt img{
  position: relative;
  // z-index: 0;
  width: 40rem;
  height: 40rem;
}
.btn-signup{
  background-color: rgb(48, 48, 48);
  color: white;
  padding: .5rem;
  border-color: $color_blue;
}
.bottom-footer-rt{
  display: flex;
  gap: 1rem;
  align-items: center;
}
#title-follow{
  color: $color_blue;
  font-weight: 800;
  font-size: 1.6rem;
}
</style>
