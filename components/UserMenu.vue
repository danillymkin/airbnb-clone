<template>
  <div class="relative">
    <div class="flex flex-row items-center gap-3">
      <div
        @click=""
        class="hidden md:block text-sm font-semibold py-3 px-4 rounded-full hover:bg-neutral-100 transition cursor-pointer"
      >
        Airbnb your home
      </div>

      <div
        @click="isOpen = !isOpen"
        class="p-4 md:py-1 md:px-2 border border-neutral-200 flex flex-row items-center gap-3 rounded-full cursor-pointer hover:shadow-md transition"
      >
        <Icon name="iconoir:menu" />

        <div class="hidden md:block">
          <Avatar />
        </div>
      </div>
    </div>

    <div
      v-if="isOpen"
      class="absolute rounded-xl shadow-md w-[40vw] md:w-3/4 bg-white overflow-hidden ring-0 top-12 text-sm"
    >
      <div class="flex flex-col cursor-pointer">
        <MenuItem @click="" label="Login" />

        <MenuItem @click="" label="Sign up" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
const isOpen = useState("isOpen", () => false);
</script>
