<template>
  <a
    v-if="context.repeatable"
    class="formulate-input-group-repeatable-remove"
    role="button"
    @click.prevent="removeItem"
    @keypress.enter="removeItem"
    v-text="`Remove`"
  />
</template>

<script>
export default {
  props: {
    context: {
      type: Object,
      required: true
    },
    removeItem: {
      type: Function,
      required: true
    }
  }
}
</script>
