<template>
  <div class="log-info-wrapper">
    <a :href="issueUrl" target="__blank" class="log-link">#{{issueNumber}}</a>
    <div class="log-text">{{issueText}}</div>
  </div>
</template>

<script>
export default {
  props: ["issueUrl", "issueNumber", "issueText"]
};
</script>

<style lang="scss">
@import "../../assets/styles/main.scss";

.log-info-wrapper {
  display: flex;
  margin-bottom: 5px;
}

.log-link {
  margin: 0 10px 0 0;
}

.log-text {
  margin: 0;
}
</style>