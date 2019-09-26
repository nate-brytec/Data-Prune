<template>
  <footer class="main-footer d-flex p-2 px-3 bg-white border-top">
    <div>
      <p class="text-center">Created by Nathaniel Senje</p>
    </div>
  </footer>
</template>

<script>
const defaultMenuItems = [
  {
    title: "Home",
    to: "#"
  },
  {
    title: "Services",
    to: "#"
  },
  {
    title: "About",
    to: "#"
  },
  {
    title: "Products",
    to: "#"
  },
  {
    title: "Blog",
    to: "#"
  }
];

export default {
  name: "main-footer",
  props: {
    /**
     * The footer menu items.
     */
    menuItems: {
      type: Array,
      default() {
        return defaultMenuItems;
      }
    },
    /**
     * The copyright information.
     */
    copyright: {
      type: String,
      default: "Copyright © 2018 DesignRevision"
    },
    /**
     * Whether the footer should be wrapped in a container, or not.
     */
    contained: {
      type: Boolean,
      default: false
    }
  }
};
</script>
