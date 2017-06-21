<template>
  <div class="layout pure-g">
    <app-sider id="app-sider"></app-sider>
    <div class="content pure-u-2-3">
      <div class="pure-g">
        <div class="pure-u-1">
          <form class="search-form pure-form">
            <input type="text" class="pure-input-rounded pure-u-5-6">
            <button type="submit" class="pure-button">Search</button>
          </form>
        </div>

      </div>
      <div class="pure-g">
        <div class="cards pure-u-1-3">
          <h1>今日更新</h1>
          <h2>5</h2>
        </div>

        <div class="cards pure-u-1-3">
          <h1>标签总数</h1>
          <h2>172</h2>
        </div>

        <div class="cards pure-u-1-3">
            <h1>工具总数</h1>
            <h2>290</h2>
        </div>
      </div>
      <div class="layout-item l-wrap pure-g">
        <div class="layout-item-screenshot content pure-u-1 u-sm-1-2">
          <a href="/layouts/blog/">
            <img src="https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=751907756,2058054255&fm=26&gp=0.jpg" class="pure-img-responsive" width="400" height="214"
                 alt="Screenshot of Blog example layout.">
          </a>
        </div>

        <div class="layout-item-content content pure-u-1 u-sm-1-2">
          <h3 class="layout-item-head">Metasploit Framework</h3>
          <p>Metasploit Framework Now lets pentest anything...</p>

          <ul class="layout-item-modules pure-g">
            <li class="layout-item-module layout-item-module-base pure-u">
              <a href="/base/">渗透框架</a>
            </li>
            <li class="layout-item-module layout-item-module-grids pure-u">
              <a href="/grids/">Ruby</a>
            </li>
            <li class="layout-item-module layout-item-module-buttons pure-u">
              <a href="/buttons/">Framework</a>
            </li>
            <li class="layout-item-module layout-item-module-menus pure-u">
              <a href="/menus/">Rapid7</a>
            </li>
          </ul>

          <p>
            <a href="/layouts/blog/" class="pure-button pure-button-primary">View</a>

            <a download="" href="/layouts/blog/download"
               onclick="return Pure.trackDownload.call(this, 'layouts', 'blog');" class="pure-button">Download</a>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import AppSider from './AppSider'

  export default {
    name: 'app-main',
    components: {
      AppSider
    }
  }
</script>


<style scoped>
  .layout {
    max-width: 92%;
    margin-right: auto;
    margin-left: auto;
    margin-top: 6rem;
    margin-bottom: 4rem;
    min-height: 30%;
  }

  .content {
    margin: 0 auto;
  }

  .search-form {
    margin-left: 3rem;
    margin-bottom: 2rem;
    margin-top: 0.5rem;
  }

  .cards {
    font-family: "Raleway", "Helvetica Neue", Helvetica, Arial, sans-serif;
    max-width: 768px;
    margin: 0 auto;
    padding: 1em;
    text-align: center;
    /* border-bottom: 1px solid #eee; */
    letter-spacing: 0.05em;
  }

  .cards h1 {
    font-size: 300%;
    font-weight: 100;
    margin: 0;
  }

  .cards h2 {
    font-size: 125%;
    font-weight: 100;
    line-height: 1.5;
    margin: 1.5rem;
    color: #666;
    letter-spacing: -0.02em;
  }

  .layout-item {
    margin-top: 2em;
    padding-top: 2em;
    border-top: 1px solid #eee;
  }
  .layout-item-screenshot {
    text-align: center;
  }
  .layout-item-head {
    margin-top: 0; /* so that the .layout-item-head lines up with the image */
  }
  .layout-item-modules {
    padding: 0;
  }
  .layout-item-module {
    margin-right: 0.5714em;
    font-size: 0.875em;
  }
  .layout-item-module-base a {
    border-left: 3px solid rgb(14, 144, 210);
  }
  .layout-item-module-grids a {
    border-left: 3px solid rgb(128, 88, 165);
  }
  .layout-item-module-forms a {
    border-left: 3px solid rgb(94, 185, 94);
  }
  .layout-item-module-buttons a {
    border-left: 3px solid rgb(221, 81, 76);
  }
  .layout-item-module-tables a {
    border-left: 3px solid rgb(243, 123, 29);
  }
  .layout-item-module-menus a {
    border-left: 3px solid rgb(250, 210, 50);
  }
  .layout-item-module a:link,
  .layout-item-module a:visited {
    text-transform: capitalize;
    color: rgb(75, 75, 75);
    padding: 0 0.5714em;
    line-height: 1.75;
    display: block;
  }

  .pure-img-responsive {
    max-width: 100%;
    height: auto;
  }



  @media (min-width: 48em) {
    .content .l-wrap {
      margin-left: -2em;
      margin-right: -2em;
    }

    .cards h1{
      font-size: 250%;
    }

    .cards h2{
      font-size: 150%;
    }

  }


  @media screen and (min-width: 35.5em) {
    .u-sm-1,
    .u-sm-1-1,
    .u-sm-1-2,
    .u-sm-1-3,
    .u-sm-2-3,
    .u-sm-1-4,
    .u-sm-3-4,
    .u-sm-1-5,
    .u-sm-2-5,
    .u-sm-3-5,
    .u-sm-4-5,
    .u-sm-5-5,
    .u-sm-1-6,
    .u-sm-5-6,
    .u-sm-1-8,
    .u-sm-3-8,
    .u-sm-5-8,
    .u-sm-7-8,
    .u-sm-1-12,
    .u-sm-5-12,
    .u-sm-7-12,
    .u-sm-11-12,
    .u-sm-1-24,
    .u-sm-2-24,
    .u-sm-3-24,
    .u-sm-4-24,
    .u-sm-5-24,
    .u-sm-6-24,
    .u-sm-7-24,
    .u-sm-8-24,
    .u-sm-9-24,
    .u-sm-10-24,
    .u-sm-11-24,
    .u-sm-12-24,
    .u-sm-13-24,
    .u-sm-14-24,
    .u-sm-15-24,
    .u-sm-16-24,
    .u-sm-17-24,
    .u-sm-18-24,
    .u-sm-19-24,
    .u-sm-20-24,
    .u-sm-21-24,
    .u-sm-22-24,
    .u-sm-23-24,
    .u-sm-24-24 {
      display: inline-block;
      *display: inline;
      zoom: 1;
      letter-spacing: normal;
      word-spacing: normal;
      vertical-align: top;
      text-rendering: auto;
    }

    .u-sm-1-24 {
      width: 4.1667%;
      *width: 4.1357%;
    }

    .u-sm-1-12,
    .u-sm-2-24 {
      width: 8.3333%;
      *width: 8.3023%;
    }

    .u-sm-1-8,
    .u-sm-3-24 {
      width: 12.5000%;
      *width: 12.4690%;
    }

    .u-sm-1-6,
    .u-sm-4-24 {
      width: 16.6667%;
      *width: 16.6357%;
    }

    .u-sm-1-5 {
      width: 20%;
      *width: 19.9690%;
    }

    .u-sm-5-24 {
      width: 20.8333%;
      *width: 20.8023%;
    }

    .u-sm-1-4,
    .u-sm-6-24 {
      width: 25%;
      *width: 24.9690%;
    }

    .u-sm-7-24 {
      width: 29.1667%;
      *width: 29.1357%;
    }

    .u-sm-1-3,
    .u-sm-8-24 {
      width: 33.3333%;
      *width: 33.3023%;
    }

    .u-sm-3-8,
    .u-sm-9-24 {
      width: 37.5000%;
      *width: 37.4690%;
    }

    .u-sm-2-5 {
      width: 40%;
      *width: 39.9690%;
    }

    .u-sm-5-12,
    .u-sm-10-24 {
      width: 41.6667%;
      *width: 41.6357%;
    }

    .u-sm-11-24 {
      width: 45.8333%;
      *width: 45.8023%;
    }

    .u-sm-1-2,
    .u-sm-12-24 {
      width: 50%;
      *width: 49.9690%;
    }

    .u-sm-13-24 {
      width: 54.1667%;
      *width: 54.1357%;
    }

    .u-sm-7-12,
    .u-sm-14-24 {
      width: 58.3333%;
      *width: 58.3023%;
    }

    .u-sm-3-5 {
      width: 60%;
      *width: 59.9690%;
    }

    .u-sm-5-8,
    .u-sm-15-24 {
      width: 62.5000%;
      *width: 62.4690%;
    }

    .u-sm-2-3,
    .u-sm-16-24 {
      width: 66.6667%;
      *width: 66.6357%;
    }

    .u-sm-17-24 {
      width: 70.8333%;
      *width: 70.8023%;
    }

    .u-sm-3-4,
    .u-sm-18-24 {
      width: 75%;
      *width: 74.9690%;
    }

    .u-sm-19-24 {
      width: 79.1667%;
      *width: 79.1357%;
    }

    .u-sm-4-5 {
      width: 80%;
      *width: 79.9690%;
    }

    .u-sm-5-6,
    .u-sm-20-24 {
      width: 83.3333%;
      *width: 83.3023%;
    }

    .u-sm-7-8,
    .u-sm-21-24 {
      width: 87.5000%;
      *width: 87.4690%;
    }

    .u-sm-11-12,
    .u-sm-22-24 {
      width: 91.6667%;
      *width: 91.6357%;
    }

    .u-sm-23-24 {
      width: 95.8333%;
      *width: 95.8023%;
    }

    .u-sm-1,
    .u-sm-1-1,
    .u-sm-5-5,
    .u-sm-24-24 {
      width: 100%;
    }
  }

  @media screen and (min-width: 48em) {
    .u-md-1,
    .u-md-1-1,
    .u-md-1-2,
    .u-md-1-3,
    .u-md-2-3,
    .u-md-1-4,
    .u-md-3-4,
    .u-md-1-5,
    .u-md-2-5,
    .u-md-3-5,
    .u-md-4-5,
    .u-md-5-5,
    .u-md-1-6,
    .u-md-5-6,
    .u-md-1-8,
    .u-md-3-8,
    .u-md-5-8,
    .u-md-7-8,
    .u-md-1-12,
    .u-md-5-12,
    .u-md-7-12,
    .u-md-11-12,
    .u-md-1-24,
    .u-md-2-24,
    .u-md-3-24,
    .u-md-4-24,
    .u-md-5-24,
    .u-md-6-24,
    .u-md-7-24,
    .u-md-8-24,
    .u-md-9-24,
    .u-md-10-24,
    .u-md-11-24,
    .u-md-12-24,
    .u-md-13-24,
    .u-md-14-24,
    .u-md-15-24,
    .u-md-16-24,
    .u-md-17-24,
    .u-md-18-24,
    .u-md-19-24,
    .u-md-20-24,
    .u-md-21-24,
    .u-md-22-24,
    .u-md-23-24,
    .u-md-24-24 {
      display: inline-block;
      *display: inline;
      zoom: 1;
      letter-spacing: normal;
      word-spacing: normal;
      vertical-align: top;
      text-rendering: auto;
    }

    .u-md-1-24 {
      width: 4.1667%;
      *width: 4.1357%;
    }

    .u-md-1-12,
    .u-md-2-24 {
      width: 8.3333%;
      *width: 8.3023%;
    }

    .u-md-1-8,
    .u-md-3-24 {
      width: 12.5000%;
      *width: 12.4690%;
    }

    .u-md-1-6,
    .u-md-4-24 {
      width: 16.6667%;
      *width: 16.6357%;
    }

    .u-md-1-5 {
      width: 20%;
      *width: 19.9690%;
    }

    .u-md-5-24 {
      width: 20.8333%;
      *width: 20.8023%;
    }

    .u-md-1-4,
    .u-md-6-24 {
      width: 25%;
      *width: 24.9690%;
    }

    .u-md-7-24 {
      width: 29.1667%;
      *width: 29.1357%;
    }

    .u-md-1-3,
    .u-md-8-24 {
      width: 33.3333%;
      *width: 33.3023%;
    }

    .u-md-3-8,
    .u-md-9-24 {
      width: 37.5000%;
      *width: 37.4690%;
    }

    .u-md-2-5 {
      width: 40%;
      *width: 39.9690%;
    }

    .u-md-5-12,
    .u-md-10-24 {
      width: 41.6667%;
      *width: 41.6357%;
    }

    .u-md-11-24 {
      width: 45.8333%;
      *width: 45.8023%;
    }

    .u-md-1-2,
    .u-md-12-24 {
      width: 50%;
      *width: 49.9690%;
    }

    .u-md-13-24 {
      width: 54.1667%;
      *width: 54.1357%;
    }

    .u-md-7-12,
    .u-md-14-24 {
      width: 58.3333%;
      *width: 58.3023%;
    }

    .u-md-3-5 {
      width: 60%;
      *width: 59.9690%;
    }

    .u-md-5-8,
    .u-md-15-24 {
      width: 62.5000%;
      *width: 62.4690%;
    }

    .u-md-2-3,
    .u-md-16-24 {
      width: 66.6667%;
      *width: 66.6357%;
    }

    .u-md-17-24 {
      width: 70.8333%;
      *width: 70.8023%;
    }

    .u-md-3-4,
    .u-md-18-24 {
      width: 75%;
      *width: 74.9690%;
    }

    .u-md-19-24 {
      width: 79.1667%;
      *width: 79.1357%;
    }

    .u-md-4-5 {
      width: 80%;
      *width: 79.9690%;
    }

    .u-md-5-6,
    .u-md-20-24 {
      width: 83.3333%;
      *width: 83.3023%;
    }

    .u-md-7-8,
    .u-md-21-24 {
      width: 87.5000%;
      *width: 87.4690%;
    }

    .u-md-11-12,
    .u-md-22-24 {
      width: 91.6667%;
      *width: 91.6357%;
    }

    .u-md-23-24 {
      width: 95.8333%;
      *width: 95.8023%;
    }

    .u-md-1,
    .u-md-1-1,
    .u-md-5-5,
    .u-md-24-24 {
      width: 100%;
    }
  }

  @media screen and (min-width: 58em) {
    .u-lg-1,
    .u-lg-1-1,
    .u-lg-1-2,
    .u-lg-1-3,
    .u-lg-2-3,
    .u-lg-1-4,
    .u-lg-3-4,
    .u-lg-1-5,
    .u-lg-2-5,
    .u-lg-3-5,
    .u-lg-4-5,
    .u-lg-5-5,
    .u-lg-1-6,
    .u-lg-5-6,
    .u-lg-1-8,
    .u-lg-3-8,
    .u-lg-5-8,
    .u-lg-7-8,
    .u-lg-1-12,
    .u-lg-5-12,
    .u-lg-7-12,
    .u-lg-11-12,
    .u-lg-1-24,
    .u-lg-2-24,
    .u-lg-3-24,
    .u-lg-4-24,
    .u-lg-5-24,
    .u-lg-6-24,
    .u-lg-7-24,
    .u-lg-8-24,
    .u-lg-9-24,
    .u-lg-10-24,
    .u-lg-11-24,
    .u-lg-12-24,
    .u-lg-13-24,
    .u-lg-14-24,
    .u-lg-15-24,
    .u-lg-16-24,
    .u-lg-17-24,
    .u-lg-18-24,
    .u-lg-19-24,
    .u-lg-20-24,
    .u-lg-21-24,
    .u-lg-22-24,
    .u-lg-23-24,
    .u-lg-24-24 {
      display: inline-block;
      *display: inline;
      zoom: 1;
      letter-spacing: normal;
      word-spacing: normal;
      vertical-align: top;
      text-rendering: auto;
    }

    .u-lg-1-24 {
      width: 4.1667%;
      *width: 4.1357%;
    }

    .u-lg-1-12,
    .u-lg-2-24 {
      width: 8.3333%;
      *width: 8.3023%;
    }

    .u-lg-1-8,
    .u-lg-3-24 {
      width: 12.5000%;
      *width: 12.4690%;
    }

    .u-lg-1-6,
    .u-lg-4-24 {
      width: 16.6667%;
      *width: 16.6357%;
    }

    .u-lg-1-5 {
      width: 20%;
      *width: 19.9690%;
    }

    .u-lg-5-24 {
      width: 20.8333%;
      *width: 20.8023%;
    }

    .u-lg-1-4,
    .u-lg-6-24 {
      width: 25%;
      *width: 24.9690%;
    }

    .u-lg-7-24 {
      width: 29.1667%;
      *width: 29.1357%;
    }

    .u-lg-1-3,
    .u-lg-8-24 {
      width: 33.3333%;
      *width: 33.3023%;
    }

    .u-lg-3-8,
    .u-lg-9-24 {
      width: 37.5000%;
      *width: 37.4690%;
    }

    .u-lg-2-5 {
      width: 40%;
      *width: 39.9690%;
    }

    .u-lg-5-12,
    .u-lg-10-24 {
      width: 41.6667%;
      *width: 41.6357%;
    }

    .u-lg-11-24 {
      width: 45.8333%;
      *width: 45.8023%;
    }

    .u-lg-1-2,
    .u-lg-12-24 {
      width: 50%;
      *width: 49.9690%;
    }

    .u-lg-13-24 {
      width: 54.1667%;
      *width: 54.1357%;
    }

    .u-lg-7-12,
    .u-lg-14-24 {
      width: 58.3333%;
      *width: 58.3023%;
    }

    .u-lg-3-5 {
      width: 60%;
      *width: 59.9690%;
    }

    .u-lg-5-8,
    .u-lg-15-24 {
      width: 62.5000%;
      *width: 62.4690%;
    }

    .u-lg-2-3,
    .u-lg-16-24 {
      width: 66.6667%;
      *width: 66.6357%;
    }

    .u-lg-17-24 {
      width: 70.8333%;
      *width: 70.8023%;
    }

    .u-lg-3-4,
    .u-lg-18-24 {
      width: 75%;
      *width: 74.9690%;
    }

    .u-lg-19-24 {
      width: 79.1667%;
      *width: 79.1357%;
    }

    .u-lg-4-5 {
      width: 80%;
      *width: 79.9690%;
    }

    .u-lg-5-6,
    .u-lg-20-24 {
      width: 83.3333%;
      *width: 83.3023%;
    }

    .u-lg-7-8,
    .u-lg-21-24 {
      width: 87.5000%;
      *width: 87.4690%;
    }

    .u-lg-11-12,
    .u-lg-22-24 {
      width: 91.6667%;
      *width: 91.6357%;
    }

    .u-lg-23-24 {
      width: 95.8333%;
      *width: 95.8023%;
    }

    .u-lg-1,
    .u-lg-1-1,
    .u-lg-5-5,
    .u-lg-24-24 {
      width: 100%;
    }
  }

  @media screen and (min-width: 75em) {
    .u-xl-1,
    .u-xl-1-1,
    .u-xl-1-2,
    .u-xl-1-3,
    .u-xl-2-3,
    .u-xl-1-4,
    .u-xl-3-4,
    .u-xl-1-5,
    .u-xl-2-5,
    .u-xl-3-5,
    .u-xl-4-5,
    .u-xl-5-5,
    .u-xl-1-6,
    .u-xl-5-6,
    .u-xl-1-8,
    .u-xl-3-8,
    .u-xl-5-8,
    .u-xl-7-8,
    .u-xl-1-12,
    .u-xl-5-12,
    .u-xl-7-12,
    .u-xl-11-12,
    .u-xl-1-24,
    .u-xl-2-24,
    .u-xl-3-24,
    .u-xl-4-24,
    .u-xl-5-24,
    .u-xl-6-24,
    .u-xl-7-24,
    .u-xl-8-24,
    .u-xl-9-24,
    .u-xl-10-24,
    .u-xl-11-24,
    .u-xl-12-24,
    .u-xl-13-24,
    .u-xl-14-24,
    .u-xl-15-24,
    .u-xl-16-24,
    .u-xl-17-24,
    .u-xl-18-24,
    .u-xl-19-24,
    .u-xl-20-24,
    .u-xl-21-24,
    .u-xl-22-24,
    .u-xl-23-24,
    .u-xl-24-24 {
      display: inline-block;
      *display: inline;
      zoom: 1;
      letter-spacing: normal;
      word-spacing: normal;
      vertical-align: top;
      text-rendering: auto;
    }

    .u-xl-1-24 {
      width: 4.1667%;
      *width: 4.1357%;
    }

    .u-xl-1-12,
    .u-xl-2-24 {
      width: 8.3333%;
      *width: 8.3023%;
    }

    .u-xl-1-8,
    .u-xl-3-24 {
      width: 12.5000%;
      *width: 12.4690%;
    }

    .u-xl-1-6,
    .u-xl-4-24 {
      width: 16.6667%;
      *width: 16.6357%;
    }

    .u-xl-1-5 {
      width: 20%;
      *width: 19.9690%;
    }

    .u-xl-5-24 {
      width: 20.8333%;
      *width: 20.8023%;
    }

    .u-xl-1-4,
    .u-xl-6-24 {
      width: 25%;
      *width: 24.9690%;
    }

    .u-xl-7-24 {
      width: 29.1667%;
      *width: 29.1357%;
    }

    .u-xl-1-3,
    .u-xl-8-24 {
      width: 33.3333%;
      *width: 33.3023%;
    }

    .u-xl-3-8,
    .u-xl-9-24 {
      width: 37.5000%;
      *width: 37.4690%;
    }

    .u-xl-2-5 {
      width: 40%;
      *width: 39.9690%;
    }

    .u-xl-5-12,
    .u-xl-10-24 {
      width: 41.6667%;
      *width: 41.6357%;
    }

    .u-xl-11-24 {
      width: 45.8333%;
      *width: 45.8023%;
    }

    .u-xl-1-2,
    .u-xl-12-24 {
      width: 50%;
      *width: 49.9690%;
    }

    .u-xl-13-24 {
      width: 54.1667%;
      *width: 54.1357%;
    }

    .u-xl-7-12,
    .u-xl-14-24 {
      width: 58.3333%;
      *width: 58.3023%;
    }

    .u-xl-3-5 {
      width: 60%;
      *width: 59.9690%;
    }

    .u-xl-5-8,
    .u-xl-15-24 {
      width: 62.5000%;
      *width: 62.4690%;
    }

    .u-xl-2-3,
    .u-xl-16-24 {
      width: 66.6667%;
      *width: 66.6357%;
    }

    .u-xl-17-24 {
      width: 70.8333%;
      *width: 70.8023%;
    }

    .u-xl-3-4,
    .u-xl-18-24 {
      width: 75%;
      *width: 74.9690%;
    }

    .u-xl-19-24 {
      width: 79.1667%;
      *width: 79.1357%;
    }

    .u-xl-4-5 {
      width: 80%;
      *width: 79.9690%;
    }

    .u-xl-5-6,
    .u-xl-20-24 {
      width: 83.3333%;
      *width: 83.3023%;
    }

    .u-xl-7-8,
    .u-xl-21-24 {
      width: 87.5000%;
      *width: 87.4690%;
    }

    .u-xl-11-12,
    .u-xl-22-24 {
      width: 91.6667%;
      *width: 91.6357%;
    }

    .u-xl-23-24 {
      width: 95.8333%;
      *width: 95.8023%;
    }

    .u-xl-1,
    .u-xl-1-1,
    .u-xl-5-5,
    .u-xl-24-24 {
      width: 100%;
    }
  }
  * {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }

  *:before,
  *:after {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }

</style>
