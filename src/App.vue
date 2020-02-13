<template>
  <div id="app">
    <h1 class="title">Peapod Rewind</h1>
    <div class="timeline--center">
        <Timeline
            :timeline-items="dataTimeline"
            :message-when-no-items="messageWhenNoItems"
            :unique-year="true"
            :color-dots="colorDots"
            order="desc"
            class="timeline-container"
        />
    </div>
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
        from: new Date(2010, 7),
        title: "Release first mobile app on apple store and google play store",
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
        from: new Date(1998, 6),
        title: "Fullfiled 1 million orders",
        description:
          `Peapod initiates service in Long Island, N.Y., with Stop &amp; Shop, and in Texas
          with Randalls and Tom Thumb
          In July, Peapod delivers its 1 millionth order, to a customer in Chicago`
      },
      {
        from: new Date(1997, 0),
        title: "IPO",
        description:`
        Peapod opens the first Stop &amp; Shop wareroom in Watertown, Mass., just
        outside Boston.
        In June, Peapod completes a successful initial public offering listing it’s shares
        on the NASDAQ.
        `
      },
      {
        from: new Date(1996, 0),
        title: "Peapod reaches a customer base of 43,200",
        description:`
        Peapod reaches a customer base of 43,200
        Peapod partners with Stop & Shop (a subsidiary of Royal Ahold) to offer
        "Peapod by Stop & Shop" in the Boston metro area
        Peapod joins the Internet, launching its own Web site: www.peapod.com
        Inc. magazine names Peapod to the "Inc. 500" ranking of the fastest-growing
        U.S. private companies.
        Peapod launches with Kroger in Columbus, OH.
        `
      },
      {
        from: new Date(1995, 0),
        title: "Launch first advertising campaign",
        description:`
        Peapod launches its first advertising campaign; the company gains 4,600
        members. (Until this time, Peapod built its customer base largely through
        word of mouth.)
        Peapod initiates service in Columbus, Ohio with The Kroger Company.
        `
      },
      {
        from: new Date(1993, 0),
        title: "Partner with Safeway in San Francisco",
        description:`
        `
      },
      {
        from: new Date(1991, 0),
        title: "Expand to Chicago",
        description:`
        With Evanston, IL, proving a success, Peapod expands its service to the
        surrounding suburbs and Chicago.
        `
      },
      {
        from: new Date(1990, 0),
        title: "Partner with Chicago-area Jewel Food Stores",
        description:`
        Peapod partners with Chicago-area Jewel Food Stores to fulfill orders. During
        the early days, Andrew, Thomas and their families do the picking and
        packing—making deliveries with their own cars.

        Peapod begins test marketing to about 400 households in Evanston, Ill. The
        company provides software and modems for customers who have to dial-in
        directly to the Peapod shopping system.
        `
      },
      {
        from: new Date(1989, 0),
        title: "Peapod Online Grocer (US) was founded in 1989 by Andrew Parkinson and Thomas Parkinson",
        description:
          `Andrew and Thomas Parkinson pioneer the online grocery delivery concept,
          establishing Peapod in Evanston, Ill. Combining backgrounds in consumer
          product marketing (Andrew was a brand manager with Proctor & Gamble and
          Kraft) and technology expertise (Thomas was the founder of a software
          company), the brothers establish Peapod as a lifestyle solution for busy
          families.
          Peapod software ran on MS-DOS as a client server application talking to an
          SCO Unix system running on a Dell 386. Disks were sold for $49.95.`
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

.timeline--center {
    display: flex;
    align-content: center;
    justify-content: center;
}

.timeline-container{
    text-align: left;
}
</style>
