<template>
  <div id="home">
    <articles>
      <banner />
    </articles>
    <intro />
    <linebutton/>
    <media/>
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
       
        
    },
  }
</script>
