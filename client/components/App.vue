<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<style>
body {
  margin: .4em;
  font-size: 2rem;
  font-family: -apple-system, BlinkMacSystemFont,
               'Avenir Next', Avenir,
               Helvetica, 'Helvetica Neue',
               Ubuntu,
               'Segoe UI', Arial,
               sans-serif;
}
.page {
  /*text-align: center;*/
  /* nesting for the need to test postcss */
  code {
    background-color: #f0f0f0;
    padding: 3px 5px;
    border-radius: 2px;
  }
}
</style>

<script>
// const webFont = require('webfontloader');
//
// // const WebFontConfig = {
// //   monotype: {
// //     projectId: '0a190ec1-8aeb-489e-905c-52340d9f21e2',
// //     // version: 0.1, // (optional, flushes the CDN cache)
// //     loadAllFonts: false, //(optional, loads all project fonts)
// //   },
// //   typekit: {
// //     id: 'abel',
// //     api: '//use.edgefonts.net',
// //   },
// //   loading() { console.log('loading'); },
// //   active() { console.log('active'); },
// //   inactive() { console.log('inactive'); },
// // };
//
// webFont.load({
//   // monotype: {
//   //   projectId: '0a190ec1-8aeb-489e-905c-52340d9f21e2',
//   //   families: ['DIN Next W01 Rounded'],
//   // },
//   typekit: {
//     id: 'source-sans-pro;lato;pt-sans;open-sans',
//     api: '//use.edgefonts.net',
//     families: ['source-sans-pro', 'lato', 'pt-sans', 'open-sans'],
//   },
//   // google: {
//   //   families: ['Droid Sans', 'Droid Serif'],
//   // },
// });
</script>
