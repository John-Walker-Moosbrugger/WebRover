<template>
  <div class="t-bio">
    <div class="t-bio__container"  v-if="!lightbox">
      <template v-for="(card, index) in team">
        <div class="t-bio__card" :key="index" @click="initLightbox(card)">
          <img :src="card.photoSM" alt="" class="card__img">
          <div class="card__overlay">
            <h4 class="card__overlay--title">{{ card.name }}</h4>
            <p class="card__overlay--role text__min">{{ card.role }}</p>
          </div>
        </div>
      </template>
    </div>
    <div class="lightbox" v-if="lightbox">
      Lightbox
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      team: [
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        },
        {
          name: 'Mike',
          role: 'President',
          photoSM: require('../assets/team/mike_sm.png'),
          photoLG: '../assets/team/mike_lg.png',
          bio: 'Mike is President and a member of the CubeRover founding team. His expertise in the space industry stems from an NSF funded project he founded and led focused on electromagnetic transportation from the lunar surface, in addition to working on Boeing’s planning team for the Space Launch System. 2016 he co-founded and led Students At Tepper for Astronautics, Rockets, and Space (STARS), a 90+ student organization at Carnegie Mellon University that con-nects passionate students with companies in the space industry. Mike joins CubeRover with an eagerness to create partnerships among the international space community and enable new opportunities. Mike is recognized in the space industry as an emerging entrepreneur. In 2018 he was selected as a delegate of the Space Generation Advisory Council’s Fusion Forum for his contribution to the global space economy. More recently, Mike was selected as one of the Top 100 Global MBAs by Poets&Quants, a renowned business publication.'
        }
      ],
      lightbox: false,
      lightboxCard: {}
    }
  },
  methods: {
    initLightbox: function (card) {
      this.lightbox = true
      this.lightboxCard = card
    }
  }
}
</script>

<style lang="scss" scoped>
.t-bio {
  &__container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 2rem;
  }

  &__card {
    position: relative;
  }
}

.card {
  &__img {
    width: 100%;
  }
  &__overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: white;
    opacity: 0;
    transition: opacity .2s ease-in-out;

    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;

    cursor: pointer;

    &:hover {
      opacity: 1;
    }

    &--title {
      font-size: 3.5rem
    }

    &--role {

    }
  }
}

.lightbox {
  height: 10rem;
  background-color: rebeccapurple;
}
</style>
