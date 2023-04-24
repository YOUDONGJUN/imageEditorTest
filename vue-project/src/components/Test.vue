<template>
  <tui-image-editor class="tui" :include-ui="useDefaultUI" :options="options"></tui-image-editor>
</template>

<script>
import 'tui-color-picker/dist/tui-color-picker.css';
import 'tui-image-editor/dist/tui-image-editor.css';
import {ImageEditor} from '@toast-ui/vue-image-editor';

export default {
  components: {
    'tui-image-editor': ImageEditor,
  },

  data() {
    return {
      useDefaultUI: true,
      options: {
        // for tui-image-editor component's "options" prop
        cssMaxWidth: 700,
        cssMaxHeight: 500,
      },
    };
  },
};
</script>

<!--<style>-->
<!--.tui {-->
<!--  width: 50% !important;-->
<!--  height: 700px;-->
<!--}-->
<!--</style>-->
