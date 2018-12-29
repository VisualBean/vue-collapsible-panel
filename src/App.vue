<template>
  <div id="app">
    <div class="columns is-vcentered has-text-centered">
      <div class="column is-4">
        <Panel title="First Panel" id="frontpage-firstpanel">Some Content</Panel>
      </div>
      <div class="column">
        <Panel title="Second Panel" id="frontpage-secondpanel">Some more Content
          <template slot="footer">
            <div class="footer-buttons">
              <button class="button is-primary is-pulled-left">Button</button>
              <button class="button is-danger is-pulled-right">Oh no!</button>
            </div>
          </template>
        </Panel>
      </div>
    </div>
  </div>
</template>

<script>
import Panel from "./components/CollapsiblePanel.vue";

export default {
  name: "app",
  components: {
    Panel
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.footer-buttons {
  padding: 0.75rem;
  width: 100%;
}
@import "~bulma";
</style>
