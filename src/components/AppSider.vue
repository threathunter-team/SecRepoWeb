<template>
  <div id="nav" class="pure-u-1-6">
    <div class="pure-menu">
      <ul class="pure-menu-list">
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">未分类<span class="email-count">(2)</span></a>
        </li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">信息收集</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">渗透测试</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">暴力破解</a></li>
        <li class="pure-menu-item"><a href="#" class="pure-menu-link">逆向工程</a></li>
        <li class="pure-menu-item pure-menu-has-children pure-menu-allow-hover">
          <a href="#" id="menuLink1" class="pure-menu-link">社会工程</a>
          <ul class="pure-menu-children">
            <li class="pure-menu-item"><a href="#" class="pure-menu-link">钓鱼</a></li>
            <li class="pure-menu-item"><a href="#" class="pure-menu-link">欺诈</a></li>
            <li class="pure-menu-item"><a href="#" class="pure-menu-link">交互</a></li>
          </ul>
        </li>

      </ul>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'app-sider'
  }
</script>


<style scoped>
  #app-sider{
    margin-right:2rem;
    text-align: center;
  }

  .pure-menu-children {
    background-color: #eee;
  }


</style>
