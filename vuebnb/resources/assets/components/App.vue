<template>
  <div>
    <header id="toolbar">
      <router-link :to="{ name: 'home' }">
        <img class="icon" src="/images/logo.png">
        <h1>vuebnb</h1>
      </router-link>
    </header>
    <router-view></router-view>
  </div>
</template>
<style>
#toolbar {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  display: flex;
  align-items: center;
  border-bottom: 1px solid #e4e4e4;
  background-color: #fff;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.1);
  z-index: 999;
}

#toolbar + * {
  margin-top: 67px;
}

#toolbar a {
  display: flex;
  align-items: center;
  text-decoration: none;
}

#toolbar .icon {
  display: inline-block;
  height: 34px;
  padding: 16px 12px 16px 24px;
}

#toolbar h1 {
  display: inline-block;
  margin: 0;
  font-size: 28px;
  color: #4fc08d;
}
</style>