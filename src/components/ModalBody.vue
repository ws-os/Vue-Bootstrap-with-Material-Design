<template>
  <div :is="tag" :class="className">
    <slot></slot>
  </div>
</template>

<script>
import classNames from 'classnames';

export default {
  props: {
    tag: {
      type: String,
      default: "div"
    },
  },
  computed: {
    className() {
      return classNames(
        'modal-body'
      );
    }
  }
};
</script>

<style scoped>

</style>
