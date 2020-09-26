<template>
  <nav class="navbar navbar-expand-lg navbar-light fixed-top">
    <a class="navbar-brand" href="#">
      <img class="adi-logo" src="../../assets/logo.png" />
      <span class="mr-4 d-md-inline d-none d-md-inline"
        >עדי זהיר - אימוני כושר אישיים וקבוצתיים</span
      >
    </a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link" v-on:click="handleClick('about')">קצת עליי</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" v-on:click="handleClick('online')"
            >ליווי Online</a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link" v-on:click="handleClick('contact')">צרו קשר</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    msg: String,
  },
  methods: {
    handleClick(link) {
      this.$emit("item-click", link);
    },
  },
};
</script>

<style scoped>
.navbar {
  background-color: white;
}

.adi-logo {
  width: 70px;
  height: 70px;
}

.nav-link {
  cursor: pointer;
}
</style>
