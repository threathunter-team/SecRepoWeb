<template>
  <div id="app">
    <app-header id="app-header"></app-header>
    <app-main id="app-main"></app-main>
    <app-footer id="app-footer"></app-footer>
  </div>
</template>

<script>
  import AppHeader from './components/AppHeader'
  import AppFooter from './components/AppFooter'
  import AppMain from './components/AppMain'

  export default {
    name: 'app',
    components: {
      AppHeader,
      AppFooter,
      AppMain
    }
  }
</script>

<style>
body {
  background-color: whitesmoke;
  line-height: 1.7em;
}

@media (min-width: 48em) {

  /* We increase the body font size */
  body {
    font-size: 16px;
  }

  /* We remove the border-separator assigned to .l-box-lrg */
  .l-box-lrg {
    border: none;
  }

}

</style>
