<template>
  <div class="toast" :class="toastData.class">
    <ui-icon class="toast__icon" :icon="toastData.icon" />
    <span>{{ toastData.message }}</span>
  </div>
</template>

<script>
import UiIcon from './UiIcon';

export default {
  name: 'TheToaster',
  components: {
    UiIcon,
  },
  props: ['toastData'],
};
</script>
