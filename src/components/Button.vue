<template>
  <button class="button" @click="$emit('click',$event)">
    <slot />
  </button>
</template>

<script lang="ts">
import Vue from "vue";

import FormItem from "./Money/FormItem.vue";
import Button from "@/components/Button.vue";
import { Component } from "vue-property-decorator";

export default class EditLabel extends Vue {}
</script>

<style lang="scss" scoped>
.button {
  background: #767676;
  color: white;
  border-radius: 4px;
  border: none;
  height: 40px;
  padding: 0 16px;
  &-wrapper {
    text-align: center;
    padding: 16px;
    margin-top: 44-16px;
  }
}
</style>