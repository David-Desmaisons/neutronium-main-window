<template>
  <transition :name="name" @after-enter="afterEnter" @after-leave="afterLeave">
    <div v-show="state === 'Opened'">
      <slot>
      </slot>
    </div>
  </transition>
</template>

<script>
const props= {
  window: {
    type: Object,
    required: true
  },
  name: String
};

export default {
  props,
  mounted() {
    this.$nextTick(()=>{
      this.window.IsListeningOpen=true
      this.window.IsListeningClose=true
    })
  },
  computed: {
    state () {
      return this.window.State.name;
    }
  },
  methods: {
    afterEnter (){
      this.window.EndOpen.Execute()
      this.$emit('afterEnter')
    },
    afterLeave (){
      this.window.CloseReady.Execute()
      this.$emit('afterLeave')
    }
  }
}
</script>