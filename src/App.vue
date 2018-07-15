<template>
  <div id="app">
    <div class="stepbox">
      <span class="stepItem now"></span>
      <span class="stepItem"></span>
      <span class="stepItem"></span>
      <span class="stepItem"></span>
    </div>
    <header>
      <h1>Create Account</h1>
      <h2>Glad to see you here!</h2>
    </header>
    <form action="">
      <label>Account</label>
      <input type="text" placeholder="example@email.con">
      <label>Password</label>
      <input type="password" placeholder="●●●●●●●●">
      <label>Comfirm Password</label>
      <input type="password" placeholder="●●●●●●●●">
      <input class="button" type="submit" value="SUBMIT & NEXT">
    </form>
  </div>
</template>

<style lang="stylus">
*
  box-sizing: border-box;
body
  margin 0
  padding 0
  font-family 'hammerhead', serif, 'Microsoft JhengHei'
header
  text-align  center
#app
  max-width 480px
  margin 0 auto
  &::before
    content ''
    height 3px
    background-color #0275D8
    display block
.stepbox
  display flex
  max-width: 240px;
  margin: 0 auto;
  margin-top: 40px;
  justify-content: space-between;
  height 2px
  background-color #BEE1FF
.stepItem
  border-resize 50%
  border: 2px solid #BEE1FF
  position: relative;
  padding: 2px;
  border-radius: 50%;
  margin-top: -7px;
  margin-bottom: -7px;
  background-color: #fff;
  width 16px
  &.now
    border: 2px solid #0275d8;
    &::after
      content ''
      background-color: #0275d8;
      border-radius: 50%;
      width: 8px;
      height: 8px;
      display: block;

    
h1
  font-size 48px
  margin-bottom 0
h2
  font-size 24px
form
  label 
    font-size 20px
    padding 10px 0
    display block
  input
    line-height: 28px;
    border 2px solid #000
    border-radius 5px
    padding 10px
    width  100%
    font-size 20px
    &::-webkit-input-placeholder
      color: #999999
    &:-moz-input-placeholder
      color: #999999
    &::-moz-placeholder
      color: #999999
    &::-ms-input-placeholder
      color: #999999
  .button
    line-height: 28px;
    background-color #BEE1FF
    border 0
    margin-top 20px
    width 100%
    padding 10px
    color #fff
    font-size 20px 





</style>
