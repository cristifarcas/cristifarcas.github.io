<template>
  <div :class="$style.header">
    <header :class="$style.headerChild" />
    <img :class="$style.logoIcon" loading="eager" alt="" src="/logo.svg" />
    <div :class="$style.childFrame">
      <b :class="$style.de">DE</b>
      <img :class="$style.chevrondownIcon" alt="" src="/chevrondown@2x.png" />
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Header",
  });
</script>
<style module>
  .headerChild {
    height: 67px;
    width: 375px;
    position: relative;
    background-color: var(--surface-white);
    box-shadow: var(--dropshadow-dropdown);
    display: none;
    max-width: 100%;
  }
  .logoIcon {
    height: 44px;
    width: 150px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
    z-index: 1;
  }
  .de {
    height: 22px;
    position: relative;
    display: inline-block;
    z-index: 1;
  }
  .chevrondownIcon {
    height: 16px;
    width: 16px;
    position: relative;
    object-fit: contain;
    z-index: 1;
  }
  .childFrame {
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs) 0px 0px;
    gap: var(--gap-6xs);
  }
  .header {
    align-self: stretch;
    background-color: var(--surface-white);
    box-shadow: var(--dropshadow-dropdown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-xs) var(--padding-4xs) var(--padding-2xs)
      var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-xl);
    max-width: 100%;
    text-align: right;
    font-size: var(--noto-sans-16-size);
    color: var(--color-black);
    font-family: var(--font-open-sans);
  }
</style>
