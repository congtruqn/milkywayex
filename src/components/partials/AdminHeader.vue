<template>
<div class="container-fluid">
  <div class="navbar-header">
    <div class="logo">
      <a href="/" class="navbar-brand1"><img src="@/assets/images/logo-dark.png"></a>
    </div>
    <div class="menu">
      <ul>
        <li><a href="#">Projects</a></li>
        <li><a href="#">Allocations</a></li>
        <li><a href="#">Dashboard</a></li>
        <li><a href="#">Quests</a></li>
      </ul>
    </div>
    <div class="connect_wallet">
      <p><a href="/" class="navbar-brand1">Connect Wallet</a></p>
    </div>
  </div>
</div>
</template>
<script>
  export default {
    name: 'AdminHeader',
    data () {
      return {
        isShow:false,
        isShowLang:false
      }
    }
  }
</script>