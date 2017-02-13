<template>
  <div class='font-showcase'>
    <div class='columns'>
      <div class='column source-sans-pro'>
        <div :class='{ "active": this.isActive }' @click='toggleActive' class='box'>
          Source Sans Pro
        </div>
      </div>
      <div class='column lato'>
        <div :class='{ "active": this.isActive }' @click='toggleActive' class='box'>
          Lato
        </div>
      </div>
      <div class='column pt-sans'>
        <div :class='{ "active": this.isActive }' @click='toggleActive' class='box'>
          PT Sans
        </div>
      </div>
      <div class='column open-sans'>
        <div :class='{ "active": this.isActive }' @click='toggleActive' class='box'>
          Open Sans
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import 'bulma/css/bulma.css';

:root {
  --main-color: red;
}

.active {
  color: white;
  background-color: green;
}

.source-sans-pro {
  font-family: 'source-sans-pro', sans-serif;
}
.lato {
  font-family: 'lato', sans-serif;
}
.pt-sans {
  font-family: 'pt-sans', sans-serif;
}
.open-sans {
  font-family: 'open-sans', sans-serif;
}
</style>

<script>
export default {
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggleActive() {
      console.log(this.isActive);
      this.isActive = !this.isActive;
    },
  },
};

const webFont = require('webfontloader');

webFont.load({
  // monotype: {
  //   projectId: '0a190ec1-8aeb-489e-905c-52340d9f21e2',
  //   families: ['DIN Next W01 Rounded'],
  // },
  typekit: {
    id: 'source-sans-pro;lato;pt-sans;open-sans',
    api: '//use.edgefonts.net',
    families: ['source-sans-pro', 'lato', 'pt-sans', 'open-sans'],
  },
  // google: {
  //   families: ['Droid Sans', 'Droid Serif'],
  // },
});

// const arr = [document.querySelector('.source-sans-pro'),
//   document.querySelector('.lato'),
//   document.querySelector('.pt-sans'),
//   document.querySelector('.open-sans')];
//
// function active(e) {
//   e.classList.toggle('is-success');
// }
//
// arr.forEach(value => value.addEventListener('click', active()));
</script>
