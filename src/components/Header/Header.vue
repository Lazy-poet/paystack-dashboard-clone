\<template>
  <nav class="nav-bar">
    <div class="navbar-title">
      <div class="toggle">
        <span
          v-show="!show"
          @click="$emit('showSidebar')"
          class="fas fa-bars"
        ></span>
        <span
          v-show="show"
          @click="$emit('showSidebar')"
          class="fas fa-times"
        ></span>
      </div>
      Get Started
    </div>
    <div class="right-side">
      <span class="test">Test Mode</span>
      <img src="../../assets/bell.svg" class="bell-icon" alt="">
      <div>
        <img src="../../assets/user.svg" clas="user-icon" alt="">
        <b class="caret"></b>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
  props: {
    show: Boolean,
  },
};
</script>

<style scoped>
.nav-bar {
  font-size: 1.2rem;
  min-height: 70px;
  max-height: 70px;
  /* width: calc(100% - 215px); */
  width: 100%;

  background-color: #fff;
  position: sticky;
  height: 70px;
  padding: 0 10px;
  top: 0;
  right: 0;
  box-sizing: border-box;
  /* transform: translateX(215px); */
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid rgba(0, 0, 0, 0.05);
  z-index: 200;
  color: #57584e;
}
.toggle{
  display: block;
  margin-right: 10px;
  width: 12px;
  height: auto;
  font-size: inherit

}
.navbar-title {
  font-size: 15px;
  font-weight: 500;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #57584E
}
.right-side {
  display: flex;
  align-items: center;
  justify-content: space-between;
  text-align: right;
  height: 40px;
  position: absolute;
  right:30px;
}
.bell-icon{
  width: 21px;
  height: 20px;
  margin-left: 25px
}
.right-side > div{
  margin-left: 25px;
  padding: 0;

}
.user-icon{
  margin-left: 10px;
  height: 21px;
  width: 21px

}
.test {
display: inline-block;
height: 30px;
line-height: 28px;
padding: 0 15px;
font-size: 12px;
letter-spacing: .2px;
border: 1px solid #e7e7e7;
color: #f05050;
border-radius: 20px;
font-weight: 500;
cursor: pointer;
}

i {
  background-color: transparent;
  color: #c1c1be;
  font-size: 20px;
  font-weight: 100;
}
.caret {
    display: inline-block;
    width: 0;
    height: 0;
    color: #919191;
    margin-left: 5px;
    vertical-align: middle;
    border-top: 4px solid;
    border-right: 4px solid transparent;
    border-left: 4px solid transparent;
}
i:not(.fa-caret-down) {
  margin-left: 25px;
}

@media (min-width: 1024px) {
  .toggle {
    display: none;
  }
  .nav-bar{
    padding: 0 30px
  }
}
</style>