<template>
  <div class="c-our-team" id="team">
    <div class="c-our-team__content">
      <div class="c-our-team__photo">
        <img src="~/static/images/index/team.png" />
      </div>
      <div class="c-our-team__text">
        <h2 class="c-our-team__header">{{ $t('Our team & history') }}</h2>
        <p>{{ $t('We\’re a {year}-year-old foundation with amazing growth and an eventful story.', { year }) }}</p>
        <div class="c-our-team__text-link">
          <a href="/foundation">{{ $t('Find out more about us!') }}</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    computed: {
      year: function() {
        return Math.floor((Date.now() - new Date('2013-02-23T18:00:00'))/(1000 * 60 * 60 * 24 * 365));
      },
    },
  };
</script>

<style lang="scss" scoped>
  @import '~/assets/_variables.scss';

  .c-our-team {
    background: $grey-bg;
    padding: 40px 0;

    &__content {
      max-width: $content-width;
      margin: 40px auto;
      display: flex;
    }

    &__photo {
      flex: 1;
      margin-right: 20px;

      img {
        width: 100%;
        border-radius: 5px;
      }
    }

    &__text {
      flex: 1;
      margin-left: 20px;

      p {
        margin: 10px 0;
      }

      &-link {
        margin: 25px 0;
        a {
          color: $cd-orange;
          font-weight: bold;
        }
      }
    }

    &__header {
      margin-top: 0;
    }
  }

  @include media-breakpoint-max(sm) {
    .c-our-team {
      &__content {
        flex-direction: column-reverse;
      }

      &__photo {
        margin: 0;
      }

      &__text {
        margin: 0 20px;
      }
    }
  }
</style>
