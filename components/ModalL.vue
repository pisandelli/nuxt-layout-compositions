<script lang="ts">
/**
   * A modal positioner
   * @name 'ModalL'
   * @version 2.0.0
   */

import { defineComponent, h } from 'vue'
import Styles from '@/assets/styles/ModalL.module.styl'

export default defineComponent({
  props: {
    tag: {
      type: String,
      default: 'div'
    }
  },
  setup(props, { slots }) {
    return () => h(props.tag, { class: Object.values(Styles) }, slots)
  }
})
</script>
