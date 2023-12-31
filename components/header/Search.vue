<template>
  <div
    class="border w-full md:w-auto py-2 rounded-full shadow-sm hover:shadow-md transition cursor-pointer"
  >
    <div class="flex flex-row items-center justify-between">
      <div class="text-sm font-semibold px-6">Anywhere</div>

      <div
        class="hidden sm:block text-sm font-semibold px-6 border-x flex-1 text-center"
      >
        Any Week
      </div>

      <div
        class="text-sm pl-6 pr-2 text-gray-600 flex flex-row items-center gap-3"
      >
        <div class="hidden sm:block">Add Guests</div>

        <div
          class="flex items-center justify-center bg-rose-500 rounded-full text-white size-8"
        >
          <Icon name="bi:search" />
        </div>
      </div>
    </div>
  </div>
</template>
