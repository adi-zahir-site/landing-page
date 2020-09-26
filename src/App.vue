<template>
  <div id="app">
    <Navbar v-on:item-click="scrollMeTo($event)" />
    <div id="content">
      <div ref="about">
        <About v-on:send-click="scrollMeTo('contact')" />
      </div>
      <div ref="online">
        <Online />
      </div>
      <div class="mt-24" ref="contact">
        <Contact />
      </div>
    </div>
  </div>
</template>

<script>
import "./assets/style.css";
import Navbar from "./components/navbar/Navbar";
import About from "./components/about/About";
import Online from "./components/online/Online";
import Contact from "./components/contact/Contact";

export default {
  name: "App",
  components: {
    Navbar,
    About,
    Online,
    Contact,
  },
  methods: {
    scrollMeTo(refName) {
      const element = this.$refs[refName];
      const top = element.offsetTop;
      window.scrollTo({ top: top - 100, behavior: "smooth" });
    },
  },
};
</script>
<style>
#app {
  direction: rtl;
  background-attachment: fixed;
  background-size: cover;
}

#content {
  margin-top: 100px;
}
</style>
