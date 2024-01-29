<template>
  <form :class="$style.blankQrAddAssetQuickF">
    <header />
    <section :class="$style.newAssetFrame">
      <div :class="$style.parentFrame">
        <h1 :class="$style.createNewAsset">Create new asset</h1>
        <div :class="$style.pleaseAddTheContainer">
          <p :class="$style.pleaseAddThe">
            Please add the details of the new asset to which the QR code is
            attached so that you can report a problem every time you scan the
            code again
          </p>
          <p :class="$style.pleaseAddThe">&nbsp;</p>
          <p :class="$style.allInputsMarkedWithAreR">
            <b :class="$style.allInputsMarked"
              >All inputs marked with * are required.</b
            >
          </p>
        </div>
      </div>
      <div :class="$style.serialBrandTypeFrameParent">
        <div :class="$style.serialBrandTypeFrame">
          <b :class="$style.serial">Serial*</b>
          <div :class="$style.timespan">
            <div :class="$style.serial123">Serial 123</div>
            <div :class="$style.advancedOptionsText">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisSerialIs">This serial is already used</b>
        </div>
        <div :class="$style.serialBrandTypeFrame">
          <b :class="$style.serial">Brand</b>
          <div :class="$style.timespan">
            <div :class="$style.addOrSelect">Add or select a type</div>
            <div :class="$style.advancedOptionsText">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisFieldIs">This field is required</b>
        </div>
        <div :class="$style.serialBrandTypeFrame">
          <b :class="$style.type">Type*</b>
          <div :class="$style.timespan">
            <div :class="$style.addOrSelect">Add or select a type</div>
            <div :class="$style.advancedOptionsText">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisFieldIs">This field is required</b>
        </div>
        <div :class="$style.siteParent">
          <b :class="$style.site">Site</b>
          <div :class="$style.timespan">
            <div :class="$style.addOrSelect">Select a site</div>
            <div :class="$style.advancedOptionsText">
              <img :class="$style.arrowsdownIcon" alt="" />
            </div>
          </div>
          <b :class="$style.thisFieldIs">This field is required</b>
        </div>
        <div :class="$style.selectAnAssetTypeParent">
          <div :class="$style.selectAnAsset">Select an asset type</div>
          <img :class="$style.vectorIcon" alt="" />
          <b :class="$style.kategoriename">Kategoriename </b>
          <div :class="$style.timespan4">
            <div :class="$style.rectangle" />
            <div :class="$style.timespanChild" />
            <img :class="$style.vectorIcon1" alt="" />
            <div :class="$style.newCategory">“New Category”</div>
            <b :class="$style.aNewItem">A new item will be created</b>
          </div>
        </div>
        <div :class="$style.rectangleParent">
          <div :class="$style.frameChild" />
          <div :class="$style.anmerkungen">Anmerkungen</div>
          <b :class="$style.anmerkungenOptional">Anmerkungen (optional)</b>
        </div>
        <div :class="$style.step2Parent">
          <div :class="$style.step2">
            <b :class="$style.takeAPicture">Take a picture</b>
            <div :class="$style.trashCanOutline1Wrapper">
              <div :class="$style.trashCanOutline1" />
            </div>
          </div>
          <div :class="$style.button">
            <div :class="$style.rectangle1" />
            <div :class="$style.dokumentAuswhlenParent">
              <b :class="$style.dokumentAuswhlen">Dokument auswählen</b>
              <img :class="$style.imageOutline1Icon" alt="" />
            </div>
          </div>
          <b :class="$style.img123jpg">img123.jpg</b>
          <img :class="$style.trashCanOutline1Icon" alt="" />
        </div>
      </div>
    </section>
    <button :class="$style.chevrondownParent" @click="onFrameButtonClick">
      <img :class="$style.chevrondownIcon" alt="" src="/chevrondown-1@2x.png" />
      <b :class="$style.openAdvancedOptions">Open advanced options</b>
    </button>
    <section
      :class="$style.longtermLoginFrame"
      @click="onLongtermLoginFrameClick"
    >
      <button :class="$style.pillLoginLong">
        <b :class="$style.saveAsset">Save {Asset} </b>
      </button>
    </section>
    <div :class="$style.toolbariphoneSe">
      <img :class="$style.backgroundIcon" alt="" />
      <div :class="$style.border" />
      <div :class="$style.symbol">􀐅</div>
      <div :class="$style.symbol1">􀉚</div>
      <div :class="$style.symbol2">􀈂</div>
      <div :class="$style.symbol3">􀆊</div>
      <div :class="$style.symbol4">􀆉</div>
    </div>
  </form>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import Header from "./header.vue";

  export default defineComponent({
    name: "BlankQRAddAssetQuickF",
    components: { Header },
    methods: {
      onFrameButtonClick() {
        this.$router.push("/blank-qr-add-asset-quick-form");
      },
      onLongtermLoginFrameClick() {
        // Please sync "Blank QR - Add Asset - Error" to the project
      },
    },
  });
</script>
<style module>
  .createNewAsset {
    margin: 0;
    width: 294px;
    height: 44px;
    position: relative;
    font-size: var(--font-size-13xl);
    font-weight: 700;
    font-family: var(--font-open-sans);
    color: var(--primary-dark);
    text-align: left;
    display: flex;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .pleaseAddThe {
    margin: 0;
    font-family: var(--font-open-sans);
  }
  .allInputsMarked {
    font-family: var(--font-open-sans);
  }
  .allInputsMarkedWithAreR {
    margin: 0;
  }
  .pleaseAddTheContainer {
    align-self: stretch;
    position: relative;
    font-size: var(--font-size-sm);
    line-height: 20px;
    color: var(--neutral-dark);
    text-align: left;
  }
  .parentFrame {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
    gap: var(--gap-5xs);
  }
  .serial {
    height: 27px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
  }
  .serial123 {
    width: 260.4px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--body-headline);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
  }
  .arrowsdownIcon {
    height: 24px;
    width: 24px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .advancedOptionsText {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
  }
  .timespan {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-xs) var(--padding-5xs);
    gap: var(--gap-xl);
  }
  .thisSerialIs {
    width: 179px;
    position: relative;
    font-size: var(--font-size-sm);
    display: none;
    font-family: var(--font-open-sans);
    color: var(--status-delete);
    text-align: left;
  }
  .serialBrandTypeFrame {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs) 0px 0px;
    gap: var(--gap-9xs);
  }
  .addOrSelect {
    width: 260.4px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--light-text);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
  }
  .thisFieldIs {
    width: 143px;
    position: relative;
    font-size: var(--font-size-sm);
    display: none;
    font-family: var(--font-open-sans);
    color: var(--status-delete);
    text-align: left;
  }
  .type {
    position: relative;
    font-size: var(--font-size-xl);
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
  }
  .site {
    height: 27px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .siteParent {
    align-self: stretch;
    display: none;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-9xs);
  }
  .selectAnAsset {
    position: absolute;
    top: 56px;
    left: 15.5px;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--light-text);
    text-align: left;
  }
  .vectorIcon {
    position: absolute;
    top: 63.6px;
    left: 302px;
    width: 12px;
    height: 5.8px;
  }
  .kategoriename {
    position: absolute;
    top: 0px;
    left: 0.5px;
    font-size: var(--noto-sans-bold-24-size);
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
  }
  .rectangle {
    position: absolute;
    top: 0px;
    left: 0px;
    border-radius: var(--br-9xs);
    background-color: var(--surface-white);
    border: 2px solid var(--neutral-light);
    box-sizing: border-box;
    width: 335px;
    height: 48px;
  }
  .timespanChild {
    position: absolute;
    top: 0px;
    left: 0px;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    box-sizing: border-box;
    width: 335px;
    height: 48px;
  }
  .vectorIcon1 {
    position: absolute;
    top: 19px;
    left: 305.8px;
    width: 13.2px;
    height: 6.6px;
  }
  .newCategory {
    position: absolute;
    top: 11px;
    left: 16px;
    font-size: var(--font-size-lg);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .aNewItem {
    position: absolute;
    top: 55px;
    left: 0px;
    font-size: var(--body-text-size);
    font-family: var(--font-open-sans);
    color: var(--green-default);
    text-align: left;
  }
  .timespan4 {
    position: absolute;
    top: 43px;
    left: 0px;
    width: 100%;
    height: 75px;
  }
  .selectAnAssetTypeParent {
    width: 335px;
    height: 118px;
    position: relative;
    display: none;
    max-width: 100%;
  }
  .frameChild {
    position: absolute;
    top: 45px;
    left: 0px;
    border-radius: var(--br-5xs);
    background-color: var(--surface-background);
    border: 0.5px solid var(--box-stroke);
    box-sizing: border-box;
    width: 335px;
    height: 116px;
  }
  .anmerkungen {
    position: absolute;
    top: 59px;
    left: 16px;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--light-text);
    text-align: left;
    display: inline-block;
    width: 302px;
    height: 95px;
  }
  .anmerkungenOptional {
    position: absolute;
    top: 0px;
    left: 4px;
    font-size: var(--noto-sans-bold-24-size);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .rectangleParent {
    width: 335px;
    height: 161px;
    position: relative;
    display: none;
    max-width: 100%;
  }
  .takeAPicture {
    align-self: stretch;
    flex: 1;
    position: relative;
    font-size: var(--noto-sans-bold-24-size);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .trashCanOutline1 {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 100%;
    overflow: hidden;
  }
  .trashCanOutline1Wrapper {
    width: 16px;
    height: 16px;
    position: relative;
  }
  .step2 {
    position: absolute;
    top: 0px;
    left: 0px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .rectangle1 {
    position: absolute;
    top: 0px;
    left: 0px;
    border-radius: var(--br-9xs);
    background-color: var(--surface-dark);
    width: 100%;
    height: 100%;
  }
  .dokumentAuswhlen {
    position: absolute;
    top: 3px;
    left: 28px;
    font-size: var(--font-size-smi);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .imageOutline1Icon {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 24px;
    height: 24px;
    overflow: hidden;
  }
  .dokumentAuswhlenParent {
    position: absolute;
    top: 13px;
    left: 84px;
    width: 171px;
    height: 24px;
  }
  .button {
    position: absolute;
    top: 39px;
    left: 0px;
    width: 100%;
    height: 48px;
  }
  .img123jpg {
    position: absolute;
    top: 99px;
    left: 0px;
    font-size: var(--body-text-size);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .trashCanOutline1Icon {
    position: absolute;
    top: 105px;
    left: 311px;
    width: 16px;
    height: 16px;
    overflow: hidden;
  }
  .step2Parent {
    align-self: stretch;
    height: 121px;
    position: relative;
    display: none;
  }
  .serialBrandTypeFrameParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .newAssetFrame {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-xl) 0px var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-xs);
    max-width: 100%;
  }
  .chevrondownIcon {
    height: 20px;
    width: 20px;
    position: relative;
    object-fit: contain;
  }
  .openAdvancedOptions {
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: center;
  }
  .chevrondownParent {
    cursor: pointer;
    border: none;
    padding: var(--padding-base) var(--padding-xl);
    background-color: var(--surface-white);
    align-self: stretch;
    border-radius: var(--br-9xs);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: 3px;
    white-space: nowrap;
  }
  .chevrondownParent:hover {
    background-color: #e6e6e6;
  }
  .saveAsset {
    height: 33px;
    position: relative;
    font-size: var(--noto-sans-bold-24-size);
    display: flex;
    font-family: var(--noto-sans-bold-24);
    color: var(--surface-white);
    text-align: center;
    align-items: center;
    justify-content: center;
  }
  .pillLoginLong {
    cursor: pointer;
    border: none;
    padding: var(--padding-4xs);
    background-color: var(--toolsense-bold-links);
    width: 298px;
    border-radius: var(--br-50xl);
    box-shadow: var(--primary-button-shadow);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    white-space: nowrap;
  }
  .pillLoginLong:hover {
    background-color: #c26100;
  }
  .longtermLoginFrame {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-base);
    opacity: 0.5;
    cursor: pointer;
  }
  .backgroundIcon {
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    max-width: 100%;
    overflow: hidden;
    max-height: 100%;
  }
  .border {
    position: absolute;
    width: 100%;
    top: 0px;
    right: 0px;
    left: 0px;
    background-color: var(--color-gray-100);
    height: 0.3px;
  }
  .symbol {
    position: absolute;
    height: 100%;
    width: calc(100% - 331px);
    top: 0px;
    left: 323px;
    font-size: var(--font-size-2xl);
    letter-spacing: -0.41px;
    line-height: 22px;
    font-family: var(--noto-sans-bold-24);
    color: var(--color-royalblue);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .symbol1 {
    position: absolute;
    height: 100%;
    width: calc(100% - 331px);
    top: 0px;
    left: 244px;
    font-size: var(--font-size-2xl);
    letter-spacing: -0.41px;
    line-height: 22px;
    font-family: var(--noto-sans-bold-24);
    color: var(--color-royalblue);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .symbol2 {
    position: absolute;
    height: 100%;
    width: calc(100% - 331px);
    top: 0px;
    left: 166px;
    font-size: var(--font-size-2xl);
    letter-spacing: -0.41px;
    line-height: 22px;
    font-family: var(--noto-sans-bold-24);
    color: var(--color-royalblue);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .symbol3 {
    position: absolute;
    height: 100%;
    width: calc(100% - 331px);
    top: 0px;
    left: 87px;
    font-size: var(--font-size-2xl);
    letter-spacing: -0.41px;
    line-height: 22px;
    font-family: var(--noto-sans-bold-24);
    color: var(--color-lightgray-100);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .symbol4 {
    position: absolute;
    height: 100%;
    width: calc(100% - 331px);
    top: 0px;
    left: 8px;
    font-size: var(--font-size-2xl);
    letter-spacing: -0.41px;
    line-height: 22px;
    font-family: var(--noto-sans-bold-24);
    color: var(--color-royalblue);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .toolbariphoneSe {
    align-self: stretch;
    height: 44px;
    position: relative;
    flex-shrink: 0;
    display: none;
  }
  .blankQrAddAssetQuickF {
    margin: 0;
    width: 376px;
    background-color: var(--surface-white);
    box-shadow: var(--dropshadow-board);
    overflow-y: auto;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 200px;
    box-sizing: border-box;
    letter-spacing: normal;
  }
</style>
