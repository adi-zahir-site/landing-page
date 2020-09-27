<template>
  <nav class="navbar navbar-expand-lg navbar-light fixed-top">
    <a class="navbar-brand">
      <a v-on:click="handleClick('about')"><img class="adi-logo float-right" src="../../assets/logo.png" /></a>
      <div class="d-inline mr-4 float-right">
        <div>עדי זהיר</div>
        <div class="font-sm">אימוני כושר אישיים וקבוצתיים</div>
        <div class="font-sm">052-2981168</div>
      </div>
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
          <a class="nav-link unselectable" v-on:click="handleClick('about')">קצת עליי</a>
        </li>
        <li class="nav-item">
          <a class="nav-link unselectable" v-on:click="handleClick('online')"
            >ליווי Online</a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link unselectable" v-on:click="handleClick('contact')">צרו קשר</a>
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
  text-align: right;
  background-color: white;
}

.adi-logo {
  cursor: pointer;
  width: 70px;
  height: 70px;
}

.font-sm {
  font-size: 10px;
}

.nav-link {
  cursor: pointer;
}
</style>
