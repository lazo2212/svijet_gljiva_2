<script setup lang="ts">
import { onMounted } from 'vue'
import { RouterLink, RouterView } from 'vue-router'
import { gsap } from 'gsap/gsap-core'
import ScrollTrigger from 'gsap/src/ScrollTrigger'

gsap.registerPlugin(ScrollTrigger)

onMounted(() => {
  const tl = gsap.timeline()
  tl.from('nav', { duration: 0.5, yPercent: -100, opacity: 0, ease: 'power1.out' })
    .from('.logo', { opacity: 0, scale: 0.8, ease: 'back' })
    .from('.link', { opacity: 0, scale: 0.8, ease: 'back', stagger: 0.1 }, '<')

  ScrollTrigger.create({
    start: 'top top',
    end: 'bottom top',
    onUpdate: (self) => {
      if (self.direction === 1) {
        gsap.to('nav', { duration: 0.5, yPercent: -100, opacity: 0, ease: 'power1.out' })
      } else {
        gsap.to('nav', { duration: 0.5, yPercent: 0, opacity: 1, ease: 'power1.out' })
      }
    }
  })
})

const year = new Date().getFullYear()
</script>

<template>
  <!-- The <router-link> component is used to create links to different routes in the application -->
  <nav>
    <RouterLink class="logo" to="/">Svijet gljiva</RouterLink>

    <div class="nav-links">
      <RouterLink class="link" to="/">Početna</RouterLink>
      <RouterLink class="link" to="/catalog">Katalog</RouterLink>
    </div>
  </nav>
  <!-- The <router-view> component will render the matched component for the given route -->
  <RouterView />

  <footer>
    <svg viewBox="0 0 1050 100" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
      <path
        d="M 0 100 
            L 150 100
            L 150 80 L 130 80 C 150 60, 170 60, 190 80 L 170 80 L 170 100
            L 300 100
            L 300 100 L 300 50 L 280 50 C 300 25, 320 25, 340 50 L 320 50 L 320 100 
            L 450 100
            L 450 70 L 430 70 C 450 30, 470 30, 490 70 L 470 70 L 470 100
            L 600 100
            L 600 90 L 590 90 C 600 30, 620 30, 630 90 L 620 90 L 620 100
            L 750 100
            L 750 50 L 730 50 C 750 10, 770 10, 790 50 L 770 50 L 770 100
            L 900 100
            L 900 70 L 880 80 C 900 10, 920 10, 940 80 L 920 70 L 920 100
            L 1050 100"
        stroke="#fff"
        stroke-width="1"
        fill="none"
      />
    </svg>
    <p>&copy; {{ year }} Svijet gljiva. Sva prava pridržana.</p>
  </footer>
</template>

<style>
.logo,
.link {
  will-change: transform, opacity;
  backface-visibility: hidden;
  transform-style: preserve-3d;
}
</style>
