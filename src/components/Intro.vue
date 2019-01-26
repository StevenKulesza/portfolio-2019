<template>
  <div class="full">
    <div id="home" class="container-fluid full">
      <h1 class="center text-center">
        <p>Hi, I'm <strong class="dark-gray-font">Steven Kulesza</strong></p>
        <vue-typed-js class="text-center" :backSpeed="20" :showCursor="false" :loop="true" :strings="['a full stack developer', 'a problem solver', 'a javascript addict']">
          <p class="text-center">and I am <span class="typing text-center"></span>.</p>
        </vue-typed-js>
        <p>Living in <strong class="dark-gray-font">Atlanta</strong> and working at <strong class="dark-gray-font"><a href="https://moxieusa.com/">Moxie</a></strong>.</p>
      </h1>
      <footer class='footer text-center'>
        <a target='_blank' href='../assets/resume-2019.pdf'>resume</a> - <a href='mailto:info@stevenkulesza.com'>email</a>
      </footer>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import VueTypedJs from 'vue-typed-js';

Vue.use(VueTypedJs);

@Component
export default class Intro extends Vue {
  @Prop() private msg!: string;
}
</script>

<style scoped lang="scss">
  $font-base:  "Raleway", sans-serif;
  $font-about:  "Droid Serif", sans-serif;

  $dark-grey:   #222426;

  $phone: "(min-width: 320px) and (max-width: 767px)";
  $tablet: "(min-width: 768px) and (max-width: 1023px)";
  $desktop: "(min-width: 1024px)";
  
@media #{$desktop} {
  #home {
    h1 {

      p {
        font-size: 42px;
        font-weight: 400;
      }

      strong {
        font-size: 46px;
      }
    }
  }
}

@media #{$tablet} {
  #home {
    h1 {

      p {
        font-size: 38px;
        font-weight: 400;
      }

      strong {
        font-size: 42px;
      }
    }
  }
}

@media #{$phone} {
  #home {
    h1 {

      p {
        font-size: 30px;
        font-weight: 400;
      }

      strong {
        font-size: 34px;
      }
    }
  }
}
.typed-element{
  display: block;
}
.dark-gray-background {
  background-color: $dark-grey;
}

.dark-gray-font {
  color: $dark-grey !important;
}

.footer {
    bottom: 30px;
    position: absolute;
    width: 100%;
}
</style>
