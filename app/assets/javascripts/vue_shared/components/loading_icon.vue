<script>
  export default {
    props: {
      label: {
        type: String,
        required: false,
        default: 'Loading',
      },

      size: {
        type: String,
        required: false,
        default: '1',
      },

      inline: {
        type: Boolean,
        required: false,
        default: false,
      },
    },

    computed: {
      rootElementType() {
        return this.inline ? 'span' : 'div';
      },
      cssClass() {
        return `fa-${this.size}x`;
      },
    },
  };
</script>
<template>
  <component
    :is="rootElementType"
    class="loading-container text-center">
    <i
      :class="cssClass"
      :aria-label="label"
      class="fa fa-spin fa-spinner"
      aria-hidden="true"
    >
    </i>
  </component>
</template>
