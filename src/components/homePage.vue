<template>
  <div class="defalutPage">
    <div class="titleText">
      <p>The 1st inLuShan CTF Game</p>
      <p>第一届“在鹿山”CTF 业余兴趣挑战赛</p>
    </div>
    <div class="startBtn">
      <t-button size="large" @click="visible = true">现在开始</t-button>
    </div>
    <t-dialog
      header="CURL"
      body="ARE YOU OK?"
      :visible.sync="visible"
      @confirm="onConfirm"
      :onConfirm="onConfirmAnother"
      :onCancel="onCancel"
      :onEscKeydown="onKeydownEsc"
      :onCloseBtnClick="onClickCloseBtn"
      :onOverlayClick="onClickOverlay"
      :onClose="close"
      :cancelBtn="null"
      :confirmBtn="null"
    ></t-dialog>
  </div>
</template>

<script>
console.log("Welcome to the 1st CTF Game hold by inLuShan");
console.log(
  "The solution to the first question is hidden in the page, and the entire page will appear hierarchical when you find this solution."
);
console.log("欢迎参加由 在鹿山 举办的第一届CTF业余兴趣挑战赛");
console.log(
  "第一题的解决方法就在这个页面中，当你找到这个可行的解决方案时，这个网页应当会被一层遮罩遮住。"
);

export default {
  name: "defalutPage",
  data() {
    return {
      visible: false,
    };
  },
  methods: {},
};
</script>

<style>
.defalutPage {
  margin-top: 200px;
}

.titleText {
  font-size: 50px;
  font-weight: bold;
  color: #2c3e50;
  margin-top: 60px;
}
</style>