<script lang="ts">
/**
   * A component that can create a
   * horizontally centered column
   * @name 'ClusterL'
   * @version 2.0.0
   */
import { defineComponent, h } from 'vue'
import Styles from '@/assets/styles/ClusterL.module.styl'

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
