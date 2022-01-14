<template>
  <section>
    <div class="item-color"
             v-for="(hex, index) in color.hex"
            :key="index"
            :style="{ 'background-color': hex}"
            >{{hex}}
    </div>
  </section>
</template>

<script>
export default {
  name: "ColorsTint",
  data() {
    return {
      colors: [
        {
          id: "1",
          title: "Tints",
          hex: [
            "#1a83c5",
            "#3391cc",
            "#4d9ed2",
            "#66acd9",
            "#80badf",
            "#99c8e5",
            "#b3d6e",
            "#cce3f2",
            "#e6f1f9",
            "#ffffff",
          ],
        },
        {
          id: "2",
          title: "Tones",
          hex: [
            "#0d76b9",
            "#1a77b2",
            "#2678ac",
            "#3379a6",
            "#407ba0",
            "#4d7c99",
            "#5a7d93",
            "#667e8d",
            "#737f86",
            "#808080",
          ],
        },
        {
          id: "3",
          title: "Shades",
          hex: [
            "#0069ac",
            "#005e99",
            "#005286",
            "#004673",
            "#003b60",
            "#002f4c",
            "#002339",
            "#001726",
            "#000c13",
            "#000000",
          ],
        },
      ],
    };
  },
};
</script>

<style>
div.color {
  width: 4rem;
  height: 4rem;
  color: #010101;
}

p {
  margin: 0;
  color: #010101;
}
</style>