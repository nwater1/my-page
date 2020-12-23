<template>
  <div id="home">
    <articles>
      <banner />
    </articles>
    
    <linebutton/>
    <articles>
      <list />
    </articles>
    <articles>
      <live />
    </articles>
    
    <blog />
    <about />

    <subscribe />

    <social />
  </div>
</template>

<script>
  export default {
    name: 'Home',

    components: {
      About: () => import('@/components/home/About'),
      Intro: () => import('@/components/home/intro'),
      Articles: () => import('@/components/home/Articles'),
      Banner: () => import('@/components/home/Banner'),
      Social: () => import('@/components/home/Social'),
      Subscribe: () => import('@/components/home/Subscribe'),
      Linebutton: () => import('@/components/home/LineButton'),
      Media: () => import('@/components/home/media'),
      blog: () => import('@/components/home/blog'),
      list: () => import('@/components/home/list'),
      live: () => import('@/components/home/live'),
       
        
    },
  }
</script>

<style scoped>
  
      
       
</style>
