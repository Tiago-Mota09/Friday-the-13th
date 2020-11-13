<template>
  <div>
    <Menu>
      <a id="menu" onclick="openMenu()">
        <span class="material-icons">menu</span>
      </a>
    </Menu>
  </div>
</template>

<style scoped>
*,
*::before,
*::after {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.material-icons {
  color: white;
  cursor: pointer;
}

/* .bm-burger-button {
  position: fixed;
  width: 36px;
  height: 30px;
  left: 36px;
  top: 36px;
  cursor: pointer;
}
.bm-burger-bars {
  background-color: #373a47;
}
.line-style {
  position: absolute;
  height: 20%;
  left: 0;
  right: 0;
}
.cross-style {
  position: absolute;
  top: 12px;
  right: 2px;
  cursor: pointer;
}
.bm-cross {
  background: #bdc3c7;
}
.bm-cross-button {
  height: 24px;
  width: 24px;
}
.bm-menu {
  height: 100%; 
  width: 0; 
  position: fixed;
  z-index: 1000; 
  top: 0;
  left: 0;
  background-color: rgb(63, 63, 65);
  overflow-x: hidden;
  padding-top: 60px; 
  transition: 0.5s; 
}
.bm-overlay {
  background: rgba(0, 0, 0, 0.3);
}
.bm-item-list {
  color: #b8b7ad;
  margin-left: 10%;
  font-size: 20px;
}
.bm-item-list > * {
  display: flex;
  text-decoration: none;
  padding: 0.7em;
}
.bm-item-list > * > span {
  margin-left: 10px;
  font-weight: 700;
  color: white;
} */
</style>

<script>
export default {
  data: () => ({
    openMenu: false,
  }),
  props: {
    menu: Boolean,
  },
  mounted() {
    this.openMenu = this.Menu;
  },
  watch: {
    menu() {
      this.openMenu = this.openMenu;
    },
  },
  methods: {
    closeMenu() {
      this.opnenMenu = false;
      this.$emit(`closed`);
    },
  },
};
</script>
