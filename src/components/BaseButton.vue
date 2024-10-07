<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  color: String,
  size: String,
  type: String,
});

//
//
//  Button de base
//
//  props:
//  - color: primary, secondary
//  - size: small, medium, large
//  - type: disabled, etc

</script>

<template>
  <button :class="[size, color, type]" :type="type">
    <slot></slot>
  </button>


</template>

<style scoped>
button {
  color: white;

  border: none;
  border-radius: 5px;
  cursor: pointer;
  border-radius: 6px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
}

.primary{
  background-color: #007bff;
  color: white;


}

.primary:hover{
  background-color: #6daff6;
}

.primary:focus{
  border: 5px solid #007bff;
}

.secondary{
  background: none;
  color: #007bff;
  border: 3px solid #007bff;

}

.secondary:hover, .secondary:focus{
  background-color: #b3d7ff;
}



.small{
  font-size: 12px;
  height: 32px;
  padding: 0px 16px;
  gap: 4px;
}

.medium{
  font-size: 16px;
  height: 48px;
  padding: 0 16px;
  gap: 8px;
}

.large{
  font-size: 20px;
  height: 56px;
  padding: 0px 24px;
  gap: 12px;

}

.disabled{
  z-index: 0;
  background-color: #d0d0d0;
  color: #6d6d6d;
  cursor: not-allowed;
}

.warning{
  background-color: #ffc107;
  color: white;
}

.warning:hover, .warning:focus{
  background-color: #ffca2c;
}


.danger{
  background-color: #dc3545;
  color: white;
}

.danger:hover, .danger:focus{
  background-color: #e4606d;
}

.disabled{
  opacity: 0.5;
}

</style>