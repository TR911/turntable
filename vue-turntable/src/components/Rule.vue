<template>
  <div class="rule-wrap">
    <h2 class="title">活动规则</h2>
    <div class="rule-con" v-html="rule"></div>
  </div>
</template>

<script>
export default {
  props: {
    rule: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss">
  .rule-wrap {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 330px;
    .title {
      font-size: 48px;
      text-align: center;
      color: #fff;
    }
    .rule-con {
      margin-top: 50px;
      padding: 0 30px;
      ul, ol {
        margin-block-start: 1em;
        margin-block-end: 1em;
        padding-inline-start: 40px;
        font-size: 32px;
        line-height: 45px;
      }
      ul {
        list-style: disc;
      }
      ol {
        list-style: decimal;
      }
      h1, h2, h3, h4, h5 {
        font-weight: 700;
      }
      h1 {
        font-size: 2em;
        margin-block-start: 0.67em;
        margin-block-end: 0.67em;
      }
      h2 {
        font-size: 1.5em;
        margin-block-start: 0.83em;
        margin-block-end: 0.83em;
      }
      h3 {
        font-size: 1.17em;
        margin-block-start: 1em;
        margin-block-end: 1em;
      }
      h4 {
        margin-block-start: 1.33em;
        margin-block-end: 1.33em;
      }
      h5 {
        margin-block-start: 1.67em;
        margin-block-end: 1.67em;
        font-size: 0.85em;
      }
      h6 {
        margin-block-start: 2.33em;
        margin-block-end: 2.33em;
      }
      p {
        margin: 1em;
      }
    }
  }
</style>
