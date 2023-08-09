<script lang="ts" setup>
import { toggleDark } from "@/composables";
</script>

<template>
  <el-menu class="el-menu-demo" mode="horizontal" background-color="var(--ep-color-primary)" text-color="#fff" active-text-color="#fff">
    <el-menu-item index="1">Element Plus</el-menu-item>
    <el-menu-item index="2">Orders</el-menu-item>
    <el-menu-item index="3" disabled>Info</el-menu-item>
    <el-sub-menu index="4">
      <template #title>Workspace</template>
      <el-menu-item index="2-1">item one</el-menu-item>
      <el-menu-item index="2-2">item two</el-menu-item>
      <el-menu-item index="2-3">item three</el-menu-item>
      <el-sub-menu index="2-4">
        <template #title>item four</template>
        <el-menu-item index="2-4-1">item one</el-menu-item>
        <el-menu-item index="2-4-2">item two</el-menu-item>
        <el-menu-item index="2-4-3">item three</el-menu-item>
      </el-sub-menu>
    </el-sub-menu>
    <el-menu-item @click="toggleDark()">
      <el-button>
        主题
      </el-button>
    </el-menu-item>
  </el-menu>
</template>
