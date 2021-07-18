<template>
  <nav role="navigation" aria-label="main navigation" :class="$style.nav">
    <!-- <nuxt-link v-for="menu in menuItem" :key="menu.title" :to="menu.url" :class="$style.navItem">
      {{ menu.title }}
    </nuxt-link> -->
  </nav>
</template>

<script>
// export default {
//   data(){
//     return{
//       isOpen: false,
//       menuItem:[
//         {
//           title:'Home',
//           url: '/'
//         },
//         {
//           title:'Markets',
//           url: '/markets'
//         },
//         {
//           title:'News',
//           url: '/news'
//         },
//         {
//           title:'Contact Us',
//           url: '/contact'
//         },
//       ]
//     }
//   },
// }
//
</script>


<style lang="scss" module>

.nav {
  @include flex();
}

</style>
