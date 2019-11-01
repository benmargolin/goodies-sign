<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,
      <br />check out the
      <a
        href="https://cli.vuejs.org"
        target="_blank"
        rel="noopener"
      >vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel"
          target="_blank"
          rel="noopener"
        >babel</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint"
          target="_blank"
          rel="noopener"
        >eslint</a>
      </li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li>
        <a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a>
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a>
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a>
      </li>
      <li>
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li>
        <a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a>
      </li>
      <li>
        <a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-devtools#vue-devtools"
          target="_blank"
          rel="noopener"
        >vue-devtools</a>
      </li>
      <li>
        <a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a>
      </li>
      <li>
        <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a>
      </li>
    </ul>

    <md-divider></md-divider>
    <div class="block">
      <h3>Number</h3>
      <md-datepicker v-model="number" md-immediately />
      <div class="value">value: {{number}}</div>
    </div>

    <md-divider></md-divider>
    <div>
      <md-card md-with-hover>
        <md-card-media>
          <img src="/assets/examples/card-image-1.jpg" alt="People" />
        </md-card-media>

        <md-card-header>
          <div class="md-title">Title goes here</div>
          <div class="md-subhead">Subtitle here</div>
        </md-card-header>

        <md-card-actions>
          <md-button>Action</md-button>
          <md-button>Action</md-button>
        </md-card-actions>

        <md-card-content>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio itaque ea, nostrum odio. Dolores, sed accusantium quasi non, voluptas eius illo quas, saepe voluptate pariatur in deleniti minus sint. Excepturi.</md-card-content>
      </md-card>
    </div>

    <md-field>
      <label>Type here!</label>
      <md-input v-model="authorName"></md-input>
      <span class="md-helper-text">Helper text</span>
    </md-field>

    <div>
      <md-button class="md-fab md-primary md-fab-bottom-right">
        <md-icon>add</md-icon>
      </md-button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data: () => ({
    selectedDate: null,
    authorName: null
  })
};
</script>

<link rel="stylesheet" href="//fonts.googleapis.com/css?family=Roboto:400,500,700,400italic|Material+Icons">

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
