<template>
  <div class="mainCard">
    <div class="avatar" :emjoi="config.emjoi">
      <img :src="config.avatarUrl" alt="" />
    </div>

    <div class="sayHi">
      <h1>
        Hi, I'm
        <span class="name" :data-text="config.name">
          {{ config.name }}
        </span>
      </h1>

      <div class="infoTags">
        <div class="tag">{{ config.infoTags.sex }}</div>
        <div class="tag">{{ config.infoTags.province }}</div>
        <div class="tag">{{ config.infoTags.school }}</div>
      </div>
    </div>
  </div>
</template>

<script setup>
import config from "../config/config.json";
</script>

<style>
@import url(../assets/css/MainCard.css);
</style>
