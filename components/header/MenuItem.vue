<template>
  <div
    @click="$emit('click')"
    class="px-4 py-3 hover:bg-neutral-100 transition font-semibold"
  >
    {{ label }}
  </div>
</template>

<script lang="ts" setup>
defineProps<{
  label: string;
}>();

defineEmits<{ click: [] }>();
</script>
