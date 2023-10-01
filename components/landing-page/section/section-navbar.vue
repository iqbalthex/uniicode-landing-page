<template>
  <nav class="w-full flex justify-between items-center px-10 py-6 text-xl bg-black shadow-md shadow-[#ccff00]">
    <div><uc-logo /></div>
    <div class="flex justify-between w-full max-w-lg">
      <a href="#" class="nav-link">Home</a>
      <a href="#" class="nav-link">About</a>
      <a href="#" class="nav-link">Member</a>
      <a href="#" class="nav-link">Partnership</a>
    </div>

    <div class="flex gap-8">
      <div class="right-button">
        <button>
          Support us
        </button>
      </div>
      <div class="right-button">
        <button>
          Join now
        </button>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">

const isNavbar = ref("");

</script>

<style scoped>

a.nav-link {
  @apply block hover:text-[#ccff00] transition;
}

.right-button > button {
  @apply px-4 py-2 h-full relative;
  border-radius: 10px;
  background: #2a3502;
  transition: all ease 0.3s;
}

.right-button {
  @apply relative p-[1px];
}

.right-button::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 10px;
  background: linear-gradient(140deg, #ccff00, #000000);
  transition: all ease 0.5s;
}

.right-button:hover > button {
  @apply text-uc-7;
  background: #ccff00;
}

</style>
