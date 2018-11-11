<template>
    <div class="news-preview">
        <h2 class="news-preview__title subtitle subtitle__purple">
            News
        </h2>
        <div class="news__articles">
            <div class="news__container">
                <img :src="news1.img" alt="" class="news__img">
                <div class="news__body">
                    <p class="text__min">{{ news1.newsType }}</p>
                    <h3 class="title__xs">{{ news1.newsTitle }}</h3>
                    <p class="text__min">{{ news1.newsPublication }}</p>
                    <p class="text__min">{{ news1.newsDate }}</p>
                </div>
            </div>
            <div class="news__container">
                <img :src="news2.img" alt="" class="news__img">
                <div class="news__body">
                    <p class="text__min">{{ news2.newsType }}</p>
                    <h3 class="title__xs">{{ news2.newsTitle }}</h3>
                    <p class="text__min">{{ news2.newsPublication }}</p>
                    <p class="text__min">{{ news2.newsDate }}</p>
                </div>
            </div>
            <div class="news__container">
                <img :src="news3.img" alt="" class="news__img">
                <div class="news__body">
                    <p class="text__min">{{ news3.newsType }}</p>
                    <h3 class="title__xs">{{ news3.newsTitle }}</h3>
                    <p class="text__min">{{ news3.newsPublication }}</p>
                    <p class="text__min">{{ news3.newsDate }}</p>
                </div>
            </div>
        </div>
        <a href="#" class="button__sm">More <img src="../assets/icons/icon_arrow-dark.png" alt="" class="icon__arrow"></a>
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
        newsTitle: 'CubeRover and Space Nation Debut the World’s First Commercial Rover',
        newsPublication: 'CubeRover',
        newsDate: 'April.24.18'
      },
      news2: {
        img: news2,
        newsType: 'Press Release',
        newsTitle: 'CubeRover and Space Nation Debut the World’s First Commercial Rover',
        newsPublication: 'CubeRover',
        newsDate: 'April.24.18'
      },
      news3: {
        img: news3,
        newsType: 'Press Release',
        newsTitle: 'CubeRover and Space Nation Debut the World’s First Commercial Rover',
        newsPublication: 'CubeRover',
        newsDate: 'April.24.18'
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

.button__sm {
    margin-top: 10rem;
}
</style>
