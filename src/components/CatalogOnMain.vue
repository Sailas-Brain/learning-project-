<template>
    <div class="catalog">
        <h2 class="catalog__title">Каталог</h2>
        <div class="catalog__wrapper">
            <div class="catalog__inner catalog__inner--one">
                <img src="@/assets/images/image 6.jpg" alt="">
                <div class="catalog__category">
                    <p>Настольные игры</p>
                </div>
            </div>
            <div class="catalog__inner catalog__inner--two">
                <img src="@/assets/images/pasha-statkevich-pinkymarmalade-wot-console-artwork-fin-2000 1.jpg" alt="">
                <div class="catalog__category">
                    <p>Варгеймы</p>
                </div>
            </div>
            <div class="catalog__inner catalog__inner--three">
                <img src="@/assets/images/image 5.jpg" alt="">
                <div class="catalog__category">
                    <p>Краски</p>
                </div>
            </div>
            <div class="catalog__inner catalog__inner--four">
                <img src="@/assets/images/image 4.jpg" alt="">
                <div class="catalog__category">
                    <p>Magic:the Cathering</p>
                </div>
            </div>
            <div class="catalog__inner catalog__inner--five">
                <img src="@/assets/images/image 7.jpg" alt="">
                <div class="catalog__category">
                    <p>Весь каталог</p>
                </div>
            </div>
          
        </div>
    </div>
</template>

<script>
  
  export default {
    name: 'catalog-on-main'
  }

</script>

<style lang="scss" scoped>

  .catalog {
    max-width: 1110px;
    margin: 0 auto;
    margin-top: 45px;

    &__title {
      font-family: "trebuchetms";
      font-weight: 700;
      font-size: 32px;
      line-height: 37px;
      color: #363636;
      margin-bottom: 22px;
      margin-top: 0;
    }

    &__wrapper {
     
      display: grid;
        grid-auto-flow: column;
        grid-template-areas: "a a b c" "a a d e";
        grid-gap: 30px;
        grid-row-gap: 1em;
    }

    &__inner {
      position: relative;
      width: 255px;
      height: 175px;
      filter: drop-shadow(5px 6px 16px rgba(42, 42, 42, 0.16));

      img {
        width: 100%;
        height: auto;
        border-radius: 9px;
      }

      &--one {
        grid-area: a;
      }

      &--two {
        grid-area: b;
      }

      &--three {
        grid-area: c;
      }

      &--four {
        grid-area: d;
      }

      &--five {
        grid-area: e;
        
        p {
          color: #F9A43F;
        }
      }

      &:first-child {
        width: 540px;
        height: 380px;
      }

    }

    &__category {
      position: absolute;
      bottom: 0;
      width: 100%;
      height: 46px;
      font-family: "trebuchetms";
      font-weight: 700;
      font-size: 18px;
      line-height: 46px;
      color: #FFFFFF;
      background: linear-gradient(180deg, #2A2A2A 0%, #2A2A2A 100%);
      border-radius: 0px 0px 9px 9px;

      p {
        margin: 0;
        margin-left: 20px;

      }

    }

  }

</style>