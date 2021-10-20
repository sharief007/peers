<template>
    <div>
      <chat-header/>
      <messages/>
      <chat-footer/>
    </div>
</template>

<script>
import ChatHeader from "@/components/ChatHeader.vue"
import Messages from "@/components/Messages.vue"
import ChatFooter from "@/components/ChatFooter.vue"

export default {
    components: {
      ChatHeader,
      Messages,
      ChatFooter
    },
    data() {
      return {
        menuItems: [
          { title: 'Click Me' },
          { title: 'Click Me' },
          { title: 'Click Me' },
          { title: 'Click Me 2' }
        ]
      }
    }
}
</script>

<style scoped>
.full-height {
    height: calc(100vh- 8rem);
}
</style>