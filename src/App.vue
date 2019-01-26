<template>
  <div id="app" class="full">
    <router-view/>
  </div>
</template>

<style lang="scss">
  $font-base:  "Raleway", sans-serif;
  $font-about:  "Droid Serif", sans-serif;

  $dark-grey:   #222426;
  $middle-blue: #00f6ed;
  $light-white: #fdfdff;
  $light-blue:  #edf9f9;
  $dark-blue:  #546a7b;
  $sidebar-color: rgba($dark-blue, .95);
  $sidebar-item-color: rgba($dark-blue, 0);

  $phone: "(min-width: 320px) and (max-width: 767px)";
  $tablet: "(min-width: 768px) and (max-width: 1023px)";
  $desktop: "(min-width: 1024px)";

  html,
  body {
    font-family: $font-base;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    -webkit-tap-highlight-color: transparent;
    height: 100%;
    min-height: 100%;
    margin:-21px 0 0;    
  }
  
  a {
    color: inherit;
    text-decoration: none !important;
  }
  .text-center {
    text-align: center;
  }
  .full {
    margin:0;
    height: 100%;
    min-height: 100%;
  }
  .center {
    left: 50%;
    position: relative;
    top: 50%;
    transform: translate(-50%, -50%);
  }

  .container-fluid {
    min-height: 100%;
    padding: 0;
  }
</style>
