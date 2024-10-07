<script>
import BaseButton from "@/components/BaseButton.vue";
import {FontAwesomeIcon} from "@fortawesome/vue-fontawesome";


export default {
  name: "AsyncButton",
  components: {
    FontAwesomeIcon,
    BaseButton,
  },
  inheritAttrs: false,
  props: {
    color: {
      type: Boolean,
      default: true,
    },
    size: {
      type: String,
      default: "small",
    },
    funct : {
      type: Function,
      default: () => {},
    },
  },
  data() {
    return {
      isPending: true,
    };
  },
  methods: {
    handleClick() {
      this.isPending = !this.isPending;
      this.funct().finally(() => {
        this.isPending = !this.isPending;
      });
    },
  },
};

</script>

<template>
  <BaseButton
    :color="color"
    :size="size"
    @click.stop.prevent="handleClick"
    :type=" isPending ? 'enabled' : 'disabled'"
  >
    <img v-if="!isPending" src="@/assets/loading.png" alt="loading" />
    <slot/>
  </BaseButton>

</template>

<style scoped>
img{
  width: 20px;
  height: 20px;
  margin-right: 10px;
  /*make it turn*/
  transform: rotate(0deg);
  animation: spin 2s linear infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}


</style>