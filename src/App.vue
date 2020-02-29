<template>
  <div class="wrapper">
    <h2>App</h2>
    <MyMain/>
  </div>
</template>

<script>
// import 変数名 from "場所"
import MyMain from "./components/Main";

// 読み込んだ Name コンポーネントを
// 使えるようにする設定
export default {
  components: {
    //MyHeader,
    MyMain
    //MyFooter
  }
};
</script>

<style>
</style>
