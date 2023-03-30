<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        {{ title }}
        <Button text="Add" color="green" />
      </v-toolbar-title>
    </v-app-bar>
  </v-app>
</template>

<script>
import Button from './Button';

export default {
  name: 'Header',
  props: {
    title: String,
  },
  components: {
    Button,
  },
};
</script>

<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
