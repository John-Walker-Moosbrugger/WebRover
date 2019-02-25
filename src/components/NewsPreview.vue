<template>
    <div class="news-preview">
        <h2 class="news-preview__title subtitle subtitle__purple">
            News
        </h2>
        <div class="news__articles">
            <a class="news__container" :href="news1.link">
                <div class="img__container">
                  <img :src="news1.img" alt="" class="news__img">
                </div>
                <div class="news__body">
                    <p class="text__min">{{ news1.newsType }}</p>
                    <h3 class="title__xs">{{ news1.newsTitle }}</h3>
                    <p class="text__min">{{ news1.newsPublication }}</p>
                    <p class="text__min">{{ news1.newsDate }}</p>
                </div>
            </a>
            <a class="news__container" :href="news2.link">
                <div class="img__container">
                  <img :src="news2.img" alt="" class="news__img">
                </div>
                <div class="news__body">
                    <p class="text__min">{{ news2.newsType }}</p>
                    <h3 class="title__xs">{{ news2.newsTitle }}</h3>
                    <p class="text__min">{{ news2.newsPublication }}</p>
                    <p class="text__min">{{ news2.newsDate }}</p>
                </div>
            </a>
            <a class="news__container" :href="news3.link">
                <div class="img__container">
                  <img :src="news3.img" alt="" class="news__img">
                </div>
                <div class="news__body">
                    <p class="text__min">{{ news3.newsType }}</p>
                    <h3 class="title__xs">{{ news3.newsTitle }}</h3>
                    <p class="text__min">{{ news3.newsPublication }}</p>
                    <p class="text__min">{{ news3.newsDate }}</p>
                </div>
            </a>
        </div>
        <!-- <router-link to="/news" class="button__sm">More <img src="../assets/icons/icon_arrow-dark.png" alt="" class="icon__arrow"></router-link> -->
    </div>
</template>

<script>
import news1 from '@/assets/news/news1.png'
import news2 from '@/assets/news/news2.png'
import news3 from '@/assets/news/news3.png'
export default {
  data () {
    return {
      news1: {
        img: news1,
        newsType: 'Press Release',
        newsTitle: 'MECO Episode: 88 CubeRover, Michael Provenzano and Andrew Horchler',
        newsPublication: 'Main Engine Cutoff',
        newsDate: 'July.30.18',
        link: 'https://mainenginecutoff.com/podcast/88'
      },
      news2: {
        img: news2,
        newsType: 'Press Release',
        newsTitle: 'CubeRover to Develop Next Generation Planetary Rovers in Luxembourg',
        newsPublication: 'Astrobotic',
        newsDate: 'September.27.18',
        link: ''
      },
      news3: {
        img: news3,
        newsType: 'Press Release',
        newsTitle: 'This Tiny Private CubeRover Could Reach the Moon by 2020',
        newsPublication: 'Space.com',
        newsDate: 'March.16.18',
        link: 'https://www.space.com/40000-astrobotic-cuberover-moon-launch-2020.html'
      }
    }
  },
  methods: {
  }
}

</script>

<style lang="scss" scoped>
.news {

    &-preview {
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;

        &__title {
        position: absolute;
        left: 4rem;
        top: 2rem;
        }
    }
    &__articles {
        width: 80%;
        display: flex;
        justify-content: space-between;
    }
    &__container {
        width: 26rem;
        height: 44rem;
        background-color: white;
        box-shadow: 0 3px 10px rgba(0, 0, 0, .2);
        display: grid;
        grid-template-rows: min-content 1fr;
        transition: .2s;
        cursor: pointer;
        color: var(--color-grey-dark);
        text-decoration: none;

        &:visited {
          color: var(--color-grey-dark);
        }

        &:hover {
            box-shadow: 0 8px 20px rgba(0, 0, 0, .25);
        }
    }
    &__img {
        width: 100%;
    }
    &__body {
        display: grid;
        grid-template-rows: min-content 1fr repeat(2, min-content);
        padding: 3rem 2rem;
    }
}

.img__container {
  overflow: hidden;
}

.button__sm {
    margin-top: 10rem;
}

@media only screen and (max-width: 1300px) {
  .news {
      &__articles {
          width: 90%;
      }
      &-preview__title {
        left: 2rem;
      }
  }
}

@media only screen and (max-width: 1000px) {
  .news {
      &__articles {
          width: 100%;
      }
      &-preview__title {
        left: -1rem;
      }
  }
}

@media only screen and (max-width: 900px) {
  .news {
    &__articles {
      max-width: 65rem;
      flex-direction: column;
    }
    &__container {
      width: 100%;
      height: 20rem;
      display: grid;
      grid-template-rows: 1fr;
      grid-template-columns: 25rem 1fr;
      margin-bottom: 3rem;
      overflow: hidden;
    }
    &__img {
      width: auto;
      height: 100%;
      margin: 0 auto;
      position: center;
      grid-column: 1 / 2;
      overflow: hidden;
    }
  }
}
@media only screen and (max-width: 650px) {
  .news {
    &__container {
      height: 18rem;
      grid-template-columns: 15rem 1fr;
    }
  }
}

@media only screen and (max-width: 560px) {

}
</style>
