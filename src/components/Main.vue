<template>

<div class="main-container">
<Header class="header" :show= "show" @showSidebar="$emit('showSidebar')"/>
<GetStarted class="get-started" />
  </div>
</template>

<script>
import Header from './Header/Header.vue';
import GetStarted from './GetStarted/GetStarted.vue'

export default {
  name: "Main",
  components: {
    Header,
    GetStarted
},
props: {
  show: Boolean,
}
}
</script>

<style scoped>
.main-container{
 /* transform: translateX(215px);
 max-width: calc(100% - 215px) */
 display: flex;
 flex-direction: column;
min-width: 960px;
height: 100%;
background: #fafafb;

}
.header{
 width: 100%;

  flex-grow: 1;
  
}

.get-started{
  /* overflow-y: auto */
 overflow-y: auto;
 overflow-x: hidden
}
</style>