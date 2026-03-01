<script setup>
import imgUrl from './assets/images/bg-14.png'
import { Search } from 'lucide-vue-next'
import { ShoppingBag } from 'lucide-vue-next'
import { Play } from 'lucide-vue-next'
import { Heart } from 'lucide-vue-next'
import Link from './components/Link.vue'
import Button from './components/Button.vue'
</script>

<template>
  <div
    class="relative h-screen w-screen bg-white overflow-hidden before:absolute before:z-10 before:inset-0 before:bg-black/15"
  >
    <!-- Header -->
    <div class="flex relative z-20 items-center justify-between px-16 py-4">
      <a href="#" class="text-white text-xl font-medium flex items-center gap-2">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-xbox"
          viewBox="0 0 16 16"
        >
          <path
            d="M7.202 15.967a8 8 0 0 1-3.552-1.26c-.898-.585-1.101-.826-1.101-1.306 0-.965 1.062-2.656 2.879-4.583C6.459 7.723 7.897 6.44 8.052 6.475c.302.068 2.718 2.423 3.622 3.531 1.43 1.753 2.088 3.189 1.754 3.829-.254.486-1.83 1.437-2.987 1.802-.954.301-2.207.429-3.239.33m-5.866-3.57C.589 11.253.212 10.127.03 8.497c-.06-.539-.038-.846.137-1.95.218-1.377 1.002-2.97 1.945-3.95.401-.417.437-.427.926-.263.595.2 1.23.638 2.213 1.528l.574.519-.313.385C4.056 6.553 2.52 9.086 1.94 10.653c-.315.852-.442 1.707-.306 2.063.091.24.007.15-.3-.319Zm13.101.195c.074-.36-.019-1.02-.238-1.687-.473-1.443-2.055-4.128-3.508-5.953l-.457-.575.494-.454c.646-.593 1.095-.948 1.58-1.25.381-.237.927-.448 1.161-.448.145 0 .654.528 1.065 1.104a8.4 8.4 0 0 1 1.343 3.102c.153.728.166 2.286.024 3.012a9.5 9.5 0 0 1-.6 1.893c-.179.393-.624 1.156-.82 1.404-.1.128-.1.127-.043-.148ZM7.335 1.952c-.67-.34-1.704-.705-2.276-.803a4 4 0 0 0-.759-.043c-.471.024-.45 0 .306-.358A7.8 7.8 0 0 1 6.47.128c.8-.169 2.306-.17 3.094-.005.85.18 1.853.552 2.418.9l.168.103-.385-.02c-.766-.038-1.88.27-3.078.853-.361.176-.676.316-.699.312a12 12 0 0 1-.654-.319Z"
          />
        </svg>
        Xbox
      </a>
      <div class="flex gap-2">
        <Link :active="true">Home</Link>
        <Link>Glasses</Link>
        <Link>Applications</Link>
        <Link>Hot deal</Link>
      </div>
      <div class="flex items-center gap-2">
        <div class="flex items-center relative w-52">
          <Search class="size-4 text-white absolute ml-3.5" />
          <input
            type="text"
            placeholder="search here"
            class="text-white text-sm w-full pl-10.5 pr-3.5 bg-black/10 rounded-full h-9 placeholder:text-white placeholder:text-sm focus:outline-0"
          />
        </div>
        <Button>Get yours</Button>
      </div>
    </div>

    <!-- Testimonials -->
    <div class="rounded-2xl absolute top-36 left-16 z-20 bg-white max-w-52 p-4 shadow-lg space-y-6">
      <p class="text-neutral-400 text-xs">
        <span class="text-2xl font-medium text-black mr-1">+150</span>Testimonials
      </p>
      <div class="text-lg">
        This things is built so well <span class="text-neutral-400">Super smooth</span>feel, totally
        worth it!
      </div>
      <div class="flex items-center justify-between">
        <div class="flex items-center -space-x-3">
          <img
            src="https://ui-avatars.com/api/?name=Elon+Musk&background=random&size=32&rounded=true"
            alt=""
          />
          <img
            src="https://ui-avatars.com/api/?name=Ival+Loic&background=random&size=32&rounded=true"
            alt=""
          />
          <img
            src="https://ui-avatars.com/api/?name=Tom+Borel&background=random&size=32&rounded=true"
            alt=""
          />
        </div>
        <div class="flex items-center gap-2 border border-neutral-200 rounded-xl h-7.5 px-1.5">
          <Heart class="size-4" />
          <span class="text-xs">50</span>
        </div>
      </div>
    </div>

    <!-- Join us -->
    <div class="space-y-4 max-w-64 absolute right-16 top-32 z-20">
      <h2 class="text-2xl text-white">Want to Join Elite Experience</h2>
      <p class="text-white text-sm">
        join our discord channel and discovers more about the controller and it space
      </p>
      <Button>
        <svg
          width="24"
          height="24"
          class="size-5"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <g class="oi-brand-facebook-fill">
            <path
              class="oi-fill"
              d="M22 12.0611C22 6.50479 17.5226 2 12.0006 2C6.47742 2 2 6.50479 2 12.0611C2 17.0829 5.65723 21.2447 10.4376 22V14.969H7.89904V12.0611H10.4376V9.84429C10.4376 7.32317 11.931 5.92982 14.2147 5.92982C15.309 5.92982 16.4537 6.1266 16.4537 6.1266V8.60278H15.192C13.9501 8.60278 13.5629 9.37794 13.5629 10.1736V12.0611H16.3361L15.8929 14.969H13.5629V22C18.3433 21.2447 22 17.0829 22 12.0611Z"
              fill="#000000"
            />
          </g>
        </svg>
        Join us
      </Button>
    </div>

    <!-- Hero -->
    <div class="absolute left-16 top-116 z-30 space-y-4">
      <h1 class="text-5xl font-medium text-white">
        XBOX Hazard <br />
        Controller
      </h1>
      <div class="flex items-center gap-2">
        <Button>
          <ShoppingBag class="size-4" />
          ByNow <span class="text-neutral-400">($200)</span>
        </Button>
        <Button variant="secondary">
          <Play class="size-4" />
          Watch video
        </Button>
      </div>
    </div>
    <img :src="imgUrl" class="absolute z-20 top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2" />
  </div>
</template>

<style lang="css"></style>
