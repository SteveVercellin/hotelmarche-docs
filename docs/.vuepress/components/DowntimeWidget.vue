<template>
  <section
    data-color-mode="auto"
    data-light-theme="light"
    data-dark-theme="dark_dimmed"
    class="my-3 pt-4 px-md-4 px-sm-2 color-bg-subtle border-md-right"
  >
    <div class="Subhead">
      <h3 class="Subhead-heading">Downtime</h3>
    </div>
    <div
      class="
        d-flex
        flex-justify-around
        my-5
        flex-content-center flex-items-stretch
      "
    >
      <div
        class="Box flex-1 text-center color-fg-accent p-3 anim-hover-grow"
        data-color-mode="auto"
        data-light-theme="light"
        data-dark-theme="dark"
      >
        <p class="f2-light">
          {{ $frontmatter.Availability.up }}<span class="text-small">%</span>
        </p>
        <span class="f5 color-fg-muted">Disponibilità</span>
      </div>
      <div
        class="Box flex-1 text-center color-fg-accent p-3 anim-hover-grow"
        data-color-mode="auto"
        data-light-theme="light"
        data-dark-theme="dark"
      >
        <p class="f2-light">{{ $frontmatter.Availability.downtimes }}</p>
        <p class="f5 color-fg-muted">
          Downtime<br /><span class="text-small color-fg-muted">{{
            $frontmatter.Availability.timedown
          }}</span>
        </p>
      </div>
    </div>
    <div
      data-color-mode="auto"
      data-light-theme="light"
      data-dark-theme="dark"
      class="container text-center color-fg-muted border rounded py-3 px-2"
    >
      <div class="text-small ml-3 my-2 color-fg-muted text-left">
        Mese Corrente:
      </div>
      <span class="diffstat flex-auto" v-for="item in items" :key="item">
        <!-- Conditional Render Based on Envent -->
        <!-- SUSPENDED -->
        <span
        style="width: 0.5625rem; height: 1rem; background-color: #ffa211; outline: 1px solid #ffa211;"
        v-if="item.Suspended == true"
        class="diffstat-block-added tooltipped tooltipped-n flex-auto"
        :aria-label="' [ Suspended ] ' + item.DownTime + ' ' + item.To"
        >

        </span>
        <!-- DOWN -->
        <span
          style="width: 0.5625rem; height: 1rem"
          v-else-if="item.Down == true"
          class="diffstat-block-deleted tooltipped tooltipped-n flex-auto"
          :aria-label="item.DownTime + ' ' + item.To"
        ></span>
        <!-- UP -->
        <span
          style="width: 0.5625rem; height: 1rem"
          v-else-if="item.Day < new Date().getDate()"
          class="diffstat-block-added tooltipped tooltipped-n flex-auto"
          :aria-label="item.Day + ' ' + $frontmatter.Availability.month"
        ></span>
        <!-- NOT CHECKED -->
        <span
          style="width: 0.5625rem; height: 1rem"
          v-else
          class="diffstat-block-neutral tooltipped tooltipped-n flex-auto"
          :aria-label="item.Day + ' ' + $frontmatter.Availability.month"
        ></span>
      </span>
    </div>
  </section>
</template>

<script>
import availabilty from "./json/downtime.json";
export default {
  name: "DowntimeWidget",
  data() {
    return {
      items: availabilty.availabilty,
    };
  },
};
</script>

<style>
</style>