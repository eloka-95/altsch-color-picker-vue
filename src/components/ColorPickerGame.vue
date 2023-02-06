
















<template>
  <div>
    <p>{{ message }}</p>
    <button v-for="color in colors" :key="color" @click="matchColor(color)">
      {{ color }}
    </button>
  </div>
</template>
<script>
  import colorPickerLogic from "../composables/Color-picker";
export default {
  setup() {
    const { colors, message, matchColor } = colorPickerLogic();
    return {
      colors,
      message,
      matchColor,
    };
  },
};

</script>



































