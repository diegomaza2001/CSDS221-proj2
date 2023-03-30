<template>
  <v-btn icon @click="onClick()" :style="{ background: color }" class="btn">
    <v-icon>mdi-magnify</v-icon> {{ text }}
  </v-btn>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      console.log('click');
    },
  },
};
</script>
