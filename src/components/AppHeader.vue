<template>
  <div class="header">
    <div class="home-menu pure-menu pure-menu-horizontal pure-menu-fixed">
      <a class="pure-menu-heading" href="">Security Tools Repository</a>

      <ul class="pure-menu-list">
        <li class="pure-menu-item pure-menu-selected"><a href="#" class="pure-menu-link">首页</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">提交工具</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">贡献榜</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">关于</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app-header',
    data () {
      return {
        title: 'SecRepo'
      }
    }
  }
</script>


<style scoped>

  .pure-menu.pure-menu-fixed {
    border-bottom: none;
    z-index: 4;
  }

  .home-menu {
    padding: .5em;
    text-align: center;
    box-shadow: 0 1px 1px rgba(0,0,0,.1);
    background: #333;
    text-transform: none;
  }


  .home-menu a {
    color: #aaa;
  }


  .home-menu .pure-menu-selected .pure-menu-link:visited {
    color: white;
  }

  .home-menu li a:hover,
  .home-menu li a:focus {
    background: none;
    border: none;
    color: #AECFE5;
  }

  .home-menu .pure-menu-heading {
    color: #fff;
    font-weight: 400;
    font-size: 120%;
  }

  home-menu .pure-menu-selected .pure-menu-link:visited {
    color: #fff;
  }

  @media (min-width: 48em) {

    /* We can align the menu header to the left, but float the
    menu items to the right. */
    .home-menu {
      text-align: left;
    }
    .home-menu ul {
      float: right;
    }

  }
</style>
