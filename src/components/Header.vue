<template>
  <div id="header">
    <!-- left -->
    <ul>
      <li>
        <router-link to="/">
          <img src="@/assets/logo.png" alt="logo" />
        </router-link>
      </li>
      <li>
        <router-link to="/">Home</router-link>
      </li>
      <li>
        <router-link to="/about">About</router-link>
      </li>
      <li>
        <router-link to="/dashboard">Dashboard</router-link>
      </li>
    </ul>

    <!-- right -->
    <ul>
      <li>
        <router-link to="/login">Login</router-link>
      </li>
      <li>
        <router-link to="/signup">Signup</router-link>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
$bg-blue: #26324d;
$font-white: #ffffff;
$font-active: #4fc08d;

#header {
  background-color: $bg-blue;
  color: $font-white;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 4%;
  box-shadow: 4px 0 16px rgba(0, 0, 0, 0.04);
  z-index: 10;

  ul {
    display: flex;
    align-items: center;

    li {
      margin-right: 16px;

      a {
        display: flex;
        align-items: center;

        &.router-link-exact-active {
          color: $font-active;
        }

        img {
          width: 160px;
        }
      }
    }
  }
}
</style>
