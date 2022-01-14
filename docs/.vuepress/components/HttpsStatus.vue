<template>
  <section
    class="py-4 px-2 color-bg-subtle border rounded"
    data-color-mode="auto"
    data-light-theme="light"
    data-dark-theme="dark_dimmed"
  >
    <div class="Subhead px-2">
      <div class="Subhead-heading">HTTPS</div>
      <div class="Subhead-actions">
        <span
          class="
            border
            color-bg-success-inverse color-text-white
            rounded
            px-2
            py-1
            text-small
          "
          >{{ https.status }}</span
        >
      </div>
      <div class="Subhead-description text-small">{{ https.label }}</div>
    </div>
    <p class="text-small px-2" v-html="https.description"></p>
    <div class="text-small px-2" v-html="https.actions"></div>
  </section>
</template>


<script>
import axios from "axios";
export default {
  data() {
    return {
      https: [],
    };
  },

  beforeMount() {
    var config = {
      method: "get",
      url: "https://energ-tech.it/wp-json/wp-site-health/v1/tests/https-status",
      headers: {
        'Authorization': 'Basic SFJTRGV2OlVqZmd4NXpsejM3VFlqdDZuZnNEckJEYw==',
      },
    };
    axios(config)
      .then((response) => {
        this.$data.https = response.data;
      })
      .then(function (response) {
        console.log(JSON.stringify(response.data));
      })
      .catch(function (error) {
        console.log(error);
      });
  },
};
</script>
