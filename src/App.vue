<template>
  <div id="app">
    <h1 class="title">Peapod Rewind</h1>
    <Timeline
      :timeline-items="dataTimeline"
      :message-when-no-items="messageWhenNoItems"
      :unique-year="true"
      :color-dots="colorDots"
      order="desc"
    />
  </div>
</template>

<script>
import Timeline from "timeline-vuejs"

export default {
  name: 'App',
  components: {
    Timeline
  },
  data: () => ({
    messageWhenNoItems: "Nothing here yet",
    colorDots: "#577926",
    dataTimeline: [
      {
        from: new Date(2020, 1, 18),
        title: "Exit Midwest Market",
        description:
          `Peapod’s online grocery delivery services in Illinois, Wisconsin, and Indiana is discontinued starting February 19.`
      },
      {
        from: new Date(2019, 0),
        title: "Open first Click and Collect to integrate with brick and mortar stores",
        description:
          ``
      },
      {
        from: new Date(2018, 7, 14),
        title: "Offer PodBag as unattended delivery packaging method",
        description:
          ``
      },
      {
        from: new Date(2018, 4),
        title: "Start Buy More Save More Promotions",
        description:
          ``
      },
      {
        from: new Date(2017, 5),
        title: "Expand filter to include four new nutrition filters: Non-GMO, Sugar-Free, Vegan, and Vegetarian.",
        description:
          ``
      },
      {
        from: new Date(2000, 5),
        title: "Royal Ahold bought 51% of Peapod's shares",
        description:
          ``
      },
      {
        from: new Date(1996, 0),
        title: "Launched its website and became one of the earliest internet start-ups",
        description:
          ``
      },
      {
        from: new Date(1989, 0),
        title: "Peapod Online Grocer (US) was founded in 1989 by Andrew Parkinson and Thomas Parkinson",
        description:
          ``
      },
    ]
  })
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.title {
    color: #577926;
    font-size: 30px;
}
</style>
