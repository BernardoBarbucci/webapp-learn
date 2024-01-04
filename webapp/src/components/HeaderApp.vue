<template>
  <header>
    <section class="container">
      <div class="logo">
        <h1>Logo</h1>
      </div>
      <div class="name">
        <h1>ShareDays</h1>
      </div>
      <div class="settings">
        <div class="menu-bar" @click="transformMenuBar">
          <div class="bar1"></div>
          <div class="bar2"></div>
          <div class="bar3"></div>
        </div>
      </div>
    </section>
  </header>
</template>

<script>
export default {
  name: 'header',
  methods: {
    transformMenuBar(event) {
      event.currentTarget.classList.toggle("change");
    }
  }
}

</script>

<style scoped>
/* menu-bar */
.menu-bar {
  display: inline-block;
  cursor: pointer;
}

.bar1,
.bar2,
.bar3 {
  width: 20px;
  height: 1.9px;
  background-color: #ffffff;
  margin: 3px 0;
  transition: 0.4s;
  border-radius: 10px;
}

.change .bar1 {
  -webkit-transform: rotate(-45deg) translate(-3px, 3.5px);
  transform: rotate(-45deg) translate(-3px, 3.5px);
}

.change .bar2 {
  opacity: 0;
}

.change .bar3 {
  -webkit-transform: rotate(45deg) translate(-3px, -4.5px);
  transform: rotate(45deg) translate(-3px, -4.5px);
}
</style>
