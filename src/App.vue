<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from './components/Home.vue'
export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Open+Sans:400,700&display=swap');
  body{
    font-family: 'Open Sans', sans-serif;
  }
  .container {
  max-width: 1150px;
  margin: 0 auto;
}
  // @import url('https://fonts.googleapis.com/css?family=Karla:400,700&display=swap');
  // body{
  //   font-family: 'Karla', sans-serif;
  // }


/* CSS resets */
html, body, div, span, applet, object, iframe, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, abbr, acronym, address, big, cite, code, del, dfn, em, img, ins, kbd, q, s, samp, small, strike, strong, sub, sup, tt, var, b, u, i, center, dl, dt, dd, ol, ul, li, fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td, article, aside, canvas, details, embed, figure, figcaption, footer, header, hgroup, menu, nav, output, ruby, section, summary, time, mark, audio, video {
    margin: 0;
        margin-bottom: 0px;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
        font-weight: inherit;
        font-size: inherit;
        font-family: inherit;
    vertical-align: baseline;
    font-family: 'Open Sans', sans-serif;
}
* {
    box-sizing: border-box;
}

  ol, ul {
    list-style: none;
  }

  img {
    max-width: 100%;
    height: auto;
  }
  article, aside, details, figcaption, figure, footer, header, hgroup, menu, nav, section {
    display: block;
}
  /* End of CSS resets */
</style>
