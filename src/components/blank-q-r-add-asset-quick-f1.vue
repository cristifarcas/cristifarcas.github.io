<template>
  <form :class="$style.blankQrAddAssetQuickF">
    <header :class="$style.header">
      <div :class="$style.headerChild" />
      <img :class="$style.logoIcon" loading="eager" alt="" src="/logo1.svg" />
      <div :class="$style.deParent">
        <b :class="$style.de">DE</b>
        <img :class="$style.chevrondownIcon" alt="" src="/chevrondown@2x.png" />
      </div>
    </header>
    <div :class="$style.blankQrAddAssetQuickFChild" />
    <div :class="$style.navigationAssetTabs1">
      <div :class="$style.navigationAssetTabs">
        <div :class="$style.navigationAssetTabs">
          <div :class="$style.navigationAssetTabsChild" />
          <div :class="$style.frameParent">
            <div :class="$style.overviewParent">
              <b :class="$style.overview">Scanned asset</b>
              <div :class="$style.frameChild" />
            </div>
            <div :class="$style.eventsParent">
              <div :class="$style.events">Events</div>
              <div :class="$style.frameItem" />
            </div>
            <div :class="$style.eventsParent">
              <div :class="$style.events">Reservations</div>
              <div :class="$style.frameInner" />
            </div>
            <div :class="$style.eventsParent">
              <div :class="$style.events">Data</div>
              <div :class="$style.lineDiv" />
            </div>
            <div :class="$style.eventsParent">
              <div :class="$style.events">Documents</div>
              <div :class="$style.frameChild1" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <section :class="$style.frameGroup">
      <div :class="$style.createNewAssetParent">
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
      <div :class="$style.chevronFrame">
        <div :class="$style.parentFrame">
          <b :class="$style.serial">Serial*</b>
          <div :class="$style.timespan">
            <div :class="$style.readyToUse">Serial 123</div>
            <div :class="$style.imageFrame">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisSerialIs">This serial is already used</b>
        </div>
        <div :class="$style.parentFrame">
          <b :class="$style.serial">Brand</b>
          <div :class="$style.timespan">
            <div :class="$style.addOrSelect">Add or select a type</div>
            <div :class="$style.imageFrame">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisFieldIs">This field is required</b>
        </div>
        <div :class="$style.parentFrame">
          <b :class="$style.type">Type*</b>
          <div :class="$style.timespan">
            <div :class="$style.addOrSelect">Add or select a type</div>
            <div :class="$style.imageFrame">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown.svg"
              />
            </div>
          </div>
          <b :class="$style.thisFieldIs">This field is required</b>
        </div>
        <div :class="$style.selectAnAssetTypeParent">
          <div :class="$style.selectAnAsset">Select an asset type</div>
          <img :class="$style.vectorIcon" alt="" />
          <b :class="$style.kategoriename">Kategoriename </b>
          <div :class="$style.timespan3">
            <div :class="$style.rectangle" />
            <div :class="$style.timespanChild" />
            <img :class="$style.vectorIcon1" alt="" />
            <div :class="$style.newCategory">“New Category”</div>
            <b :class="$style.aNewItem">A new item will be created</b>
          </div>
        </div>
        <div :class="$style.rectangleParent">
          <div :class="$style.rectangleDiv" />
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
              <input :class="$style.imageOutline1" type="checkbox" />
            </div>
          </div>
          <b :class="$style.img123jpg">img123.jpg</b>
          <img :class="$style.trashCanOutline1Icon" alt="" />
        </div>
      </div>
    </section>
    <button :class="$style.loginButtonFrame" @click="onLoginButtonFrameClick">
      <img :class="$style.chevronupIcon" alt="" src="/chevronup@2x.png" />
      <b :class="$style.closeAdvancedOptions">Close advanced options</b>
    </button>
    <section :class="$style.textFrame">
      <div :class="$style.iMEIBLEDetails">
        <div :class="$style.iMEI">
          <div :class="$style.bLETagID">
            <div :class="$style.site">
              <b :class="$style.site1">Site</b>
              <div :class="$style.timespan">
                <div :class="$style.addOrSelect">Select a site</div>
                <div :class="$style.imageFrame">
                  <img
                    :class="$style.arrowsdownIcon"
                    alt=""
                    src="/arrowsdown-3.svg"
                  />
                </div>
              </div>
              <b :class="$style.thisFieldIs">This field is required</b>
            </div>
            <div :class="$style.iMEITimespan">
              <b :class="$style.imei">IMEI</b>
              <div :class="$style.timespan5">
                <input
                  :class="$style.ddMmYyyy"
                  placeholder="IMEI"
                  type="text"
                />
                <img :class="$style.calendarIcon" alt="" />
              </div>
            </div>
            <div :class="$style.iMEITimespan">
              <b :class="$style.bleTagId">BLE Tag ID</b>
              <div :class="$style.timespan5">
                <input
                  :class="$style.ddMmYyyy"
                  placeholder="BLE Tag ID"
                  type="text"
                />
                <img :class="$style.calendarIcon" alt="" />
              </div>
            </div>
            <div :class="$style.selectAnAssetTypeParent">
              <div :class="$style.selectAnAsset">Select an asset type</div>
              <img :class="$style.vectorIcon" alt="" />
              <b :class="$style.kategoriename">Kategoriename </b>
              <div :class="$style.timespan3">
                <div :class="$style.rectangle" />
                <div :class="$style.timespanChild" />
                <img :class="$style.vectorIcon1" alt="" />
                <div :class="$style.newCategory">“New Category”</div>
                <b :class="$style.aNewItem">A new item will be created</b>
              </div>
            </div>
            <div :class="$style.rectangleParent">
              <div :class="$style.rectangleDiv" />
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
                  <input :class="$style.imageOutline1" type="checkbox" />
                </div>
              </div>
              <b :class="$style.img123jpg">img123.jpg</b>
              <img :class="$style.trashCanOutline1Icon" alt="" />
            </div>
          </div>
        </div>
        <div :class="$style.quantity">
          <b :class="$style.notes">Notes</b>
          <textarea
            :class="$style.costcenter"
            placeholder="Add a note"
            rows="5"
            cols="17"
          />
        </div>
      </div>
      <div :class="$style.warrantyPeriod">
        <div :class="$style.ownershipType">
          <b :class="$style.assetChecks">Asset checks</b>
          <img
            :class="$style.chevronupIcon"
            alt=""
            src="/chevrondown-11@2x.png"
          />
        </div>
        <div :class="$style.submenu">
          <div :class="$style.addAssetForm">
            <b :class="$style.notes">Name</b>
            <div :class="$style.timespan8">
              <input :class="$style.ddMmYyyy" placeholder="Name" type="text" />
              <img :class="$style.calendarIcon" alt="" />
            </div>
          </div>
          <div :class="$style.site">
            <b :class="$style.interval">Interval</b>
            <div :class="$style.timespan9">
              <input :class="$style.input" placeholder="12" type="text" />
              <div :class="$style.chevronpreviousParent">
                <img
                  :class="$style.chevronpreviousIcon"
                  alt=""
                  src="/chevronprevious.svg"
                />
                <img
                  :class="$style.chevronpreviousIcon"
                  alt=""
                  src="/chevronnext.svg"
                />
              </div>
            </div>
          </div>
          <div :class="$style.site">
            <b :class="$style.lastMaintenance">Last Maintenance*</b>
            <div :class="$style.timespan10">
              <input
                :class="$style.ddMmYyyy"
                placeholder="DD-MM-YYYY"
                type="text"
              />
              <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
            </div>
          </div>
          <div :class="$style.site">
            <b :class="$style.nextMaintenance">Next Maintenance*</b>
            <div :class="$style.timespan11">
              <input
                :class="$style.ddMmYyyy"
                placeholder="DD-MM-YYYY"
                type="text"
              />
              <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
            </div>
            <b :class="$style.thisFieldIs3">This field is required</b>
          </div>
          <div :class="$style.selectAnAssetTypeParent">
            <div :class="$style.selectAnAsset">Select an asset type</div>
            <img :class="$style.vectorIcon" alt="" />
            <b :class="$style.kategoriename">Kategoriename </b>
            <div :class="$style.timespan3">
              <div :class="$style.rectangle" />
              <div :class="$style.timespanChild" />
              <img :class="$style.vectorIcon1" alt="" />
              <div :class="$style.newCategory">“New Category”</div>
              <b :class="$style.aNewItem">A new item will be created</b>
            </div>
          </div>
          <div :class="$style.rectangleParent">
            <div :class="$style.rectangleDiv" />
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
      </div>
      <div :class="$style.textFrame">
        <div :class="$style.ownershipType">
          <b :class="$style.assetChecks">Maintenance</b>
          <img
            :class="$style.chevronupIcon"
            alt=""
            src="/chevrondown-11@2x.png"
          />
        </div>
        <div :class="$style.submenu">
          <div :class="$style.addAssetForm">
            <b :class="$style.interval">Interval</b>
            <div :class="$style.timespan5">
              <input :class="$style.ddMmYyyy" placeholder="12" type="text" />
              <img :class="$style.calendarIcon" alt="" />
            </div>
          </div>
          <div :class="$style.site">
            <b :class="$style.lastMaintenance">Last Maintenance*</b>
            <div :class="$style.timespan11">
              <input
                :class="$style.ddMmYyyy"
                placeholder="DD-MM-YYYY"
                type="text"
              />
              <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
            </div>
          </div>
          <div :class="$style.site">
            <b :class="$style.nextMaintenance">Next Maintenance*</b>
            <div :class="$style.timespan11">
              <input
                :class="$style.ddMmYyyy"
                placeholder="DD-MM-YYYY"
                type="text"
              />
              <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
            </div>
            <b :class="$style.thisFieldIs3">This field is required</b>
          </div>
          <div :class="$style.selectAnAssetTypeParent">
            <div :class="$style.selectAnAsset">Select an asset type</div>
            <img :class="$style.vectorIcon" alt="" />
            <b :class="$style.kategoriename">Kategoriename </b>
            <div :class="$style.timespan3">
              <div :class="$style.rectangle" />
              <div :class="$style.timespanChild" />
              <img :class="$style.vectorIcon1" alt="" />
              <div :class="$style.newCategory">“New Category”</div>
              <b :class="$style.aNewItem">A new item will be created</b>
            </div>
          </div>
          <div :class="$style.rectangleParent">
            <div :class="$style.rectangleDiv" />
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
      </div>
    </section>
    <section :class="$style.warrantyEnd">
      <div :class="$style.ownershipTypeLabel">
        <b :class="$style.inventoryDetails">Inventory details</b>
      </div>
      <div :class="$style.availabilityInfo">
        <div :class="$style.site">
          <b :class="$style.assetAvailability1">Asset Availability</b>
          <div :class="$style.timespan17">
            <div :class="$style.readyToUse">Ready to use (default)</div>
            <div :class="$style.imageFrame">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown-3.svg"
              />
            </div>
          </div>
        </div>
        <div :class="$style.addAssetForm">
          <b :class="$style.inventoryNumber">Inventory number</b>
          <div :class="$style.timespan8">
            <input
              :class="$style.ddMmYyyy"
              placeholder="Inventory number"
              type="text"
            />
            <img :class="$style.calendarIcon" alt="" />
          </div>
        </div>
        <div :class="$style.site">
          <b :class="$style.quantity1">Quantity</b>
          <div :class="$style.timespan9">
            <input
              :class="$style.quantity2"
              placeholder="Quantity"
              type="text"
            />
            <div :class="$style.chevronpreviousParent">
              <img
                :class="$style.chevronpreviousIcon"
                alt=""
                src="/chevronprevious.svg"
              />
              <img
                :class="$style.chevronpreviousIcon"
                alt=""
                src="/chevronnext.svg"
              />
            </div>
          </div>
        </div>
        <div :class="$style.addAssetForm">
          <b :class="$style.floorRoom1">Floor & Room</b>
          <div :class="$style.timespan8">
            <input
              :class="$style.floorRoom2"
              placeholder="Floor & Room"
              type="text"
            />
            <img :class="$style.calendarIcon" alt="" />
          </div>
        </div>
        <div :class="$style.addAssetForm">
          <b :class="$style.costCenter3">Cost center</b>
          <div :class="$style.timespan8">
            <input
              :class="$style.floorRoom2"
              placeholder="Cost center"
              type="text"
            />
            <img :class="$style.calendarIcon" alt="" />
          </div>
        </div>
      </div>
    </section>
    <section :class="$style.assetQuantity">
      <div :class="$style.ownershipTypeWrapper">
        <b :class="$style.ownershipType1">Ownership type</b>
      </div>
      <div :class="$style.frameContainer">
        <div :class="$style.site">
          <b :class="$style.ownershipType2">Ownership type</b>
          <div :class="$style.timespan17">
            <div :class="$style.ownershipType3">Ownership type</div>
            <div :class="$style.imageFrame">
              <img
                :class="$style.arrowsdownIcon"
                alt=""
                src="/arrowsdown-3.svg"
              />
            </div>
          </div>
        </div>
        <div :class="$style.checkedParent">
          <img
            :class="$style.checkedIcon"
            loading="eager"
            alt=""
            src="/checked.svg"
          />
          <div :class="$style.lowValueAsset">Low-value asset</div>
        </div>
      </div>
      <div :class="$style.site">
        <b :class="$style.acquisitionDate1">Acquisition date</b>
        <div :class="$style.timespan23">
          <input
            :class="$style.ddMmYyyy4"
            placeholder="DD-MM-YYYY"
            type="text"
          />
          <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
        </div>
      </div>
      <div :class="$style.site">
        <b :class="$style.invoiceNumber">Invoice number</b>
        <div :class="$style.timespan24">
          <input
            :class="$style.costCenter5"
            placeholder="Cost center"
            type="text"
          />
          <img :class="$style.calendarIcon" alt="" />
        </div>
      </div>
      <div :class="$style.site">
        <b :class="$style.warrantyStart1">Warranty start</b>
        <div :class="$style.timespan23">
          <input
            :class="$style.ddMmYyyy4"
            placeholder="DD-MM-YYYY"
            type="text"
          />
          <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
        </div>
      </div>
      <div :class="$style.site">
        <b :class="$style.warrantyPeriodIn">Warranty period (in months)</b>
        <div :class="$style.timespan9">
          <input :class="$style.input1" placeholder="12" type="text" />
          <div :class="$style.chevronpreviousParent">
            <img
              :class="$style.chevronpreviousIcon"
              alt=""
              src="/chevronprevious.svg"
            />
            <img
              :class="$style.chevronpreviousIcon"
              alt=""
              src="/chevronnext.svg"
            />
          </div>
        </div>
      </div>
      <div :class="$style.site">
        <b :class="$style.warrantyEnd1">Warranty end</b>
        <div :class="$style.timespan23">
          <input
            :class="$style.ddMmYyyy4"
            placeholder="DD-MM-YYYY"
            type="text"
          />
          <img :class="$style.calendarIcon3" alt="" src="/calendar.svg" />
        </div>
      </div>
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
    <section :class="$style.frameSection">
      <div :class="$style.addDocumentsWrapper">
        <b :class="$style.addDocuments">Add documents</b>
      </div>
      <button :class="$style.button4">
        <div :class="$style.rectangle8" />
        <img
          :class="$style.imageOutline1Icon2"
          alt=""
          src="/imageoutline-1-4.svg"
        />
        <b :class="$style.dokumentAuswhlen4">Dokument auswählen</b>
      </button>
      <div :class="$style.trashCan">
        <b :class="$style.img123jpg4">img123.jpg</b>
        <img
          :class="$style.trashCanOutline1Icon4"
          loading="eager"
          alt=""
          src="/trashcanoutline-1-4.svg"
        />
      </div>
    </section>
    <section :class="$style.loginButton" @click="onLoginButtonClick">
      <footer :class="$style.pillLoginLong">
        <h3 :class="$style.saveAsset">Save {Asset}</h3>
      </footer>
    </section>
  </form>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "BlankQRAddAssetQuickF1",
    methods: {
      onLoginButtonFrameClick() {
        this.$router.push("/");
      },
      onLoginButtonClick() {
        // Please sync "Blank QR - Add Asset - Error" to the project
      },
    },
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
    font-size: var(--noto-sans-16-size);
    display: inline-block;
    font-family: var(--font-open-sans);
    color: var(--color-black);
    text-align: right;
    z-index: 1;
  }
  .chevrondownIcon {
    height: 16px;
    width: 16px;
    position: relative;
    object-fit: contain;
    z-index: 1;
  }
  .deParent {
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: flex-start;
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
    padding: var(--padding-xs) 10px var(--padding-2xs) var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-xl);
    top: 0;
    z-index: 99;
    position: sticky;
    max-width: 100%;
  }
  .blankQrAddAssetQuickFChild {
    align-self: stretch;
    position: relative;
    background-color: var(--surface-white);
    box-shadow: var(--dropshadow-dropdown);
    height: 67px;
    display: none;
  }
  .navigationAssetTabsChild {
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0%;
    right: 0%;
    bottom: 0%;
    left: 0%;
    background-color: #d8d5d2;
  }
  .overview {
    position: absolute;
    top: 13.64%;
    left: 0%;
    font-size: var(--body-text-size);
    line-height: 18.5px;
    font-family: var(--body-text);
    color: var(--body-headline);
    text-align: center;
  }
  .frameChild {
    position: absolute;
    height: 13.64%;
    width: 69.7%;
    top: 0%;
    right: 12.12%;
    bottom: 86.36%;
    left: 18.18%;
    background-color: var(--body-headline);
    border-top: 3px solid var(--body-headline);
    box-sizing: border-box;
  }
  .overviewParent {
    height: 22px;
    flex: 1;
    position: relative;
  }
  .events {
    position: absolute;
    font-size: var(--body-text-size);
    line-height: 18.5px;
    font-family: var(--body-text);
    color: var(--body-headline);
    text-align: center;
    display: none;
  }
  .frameItem {
    position: absolute;
    background-color: var(--body-headline);
    border-top: 3px solid var(--body-headline);
    box-sizing: border-box;
    width: 59px;
    height: 3px;
    display: none;
  }
  .eventsParent {
    height: 0px;
    width: 0px;
    position: relative;
  }
  .frameInner {
    position: absolute;
    background-color: var(--body-headline);
    border-top: 3px solid var(--body-headline);
    box-sizing: border-box;
    width: 96px;
    height: 3px;
    display: none;
  }
  .lineDiv {
    position: absolute;
    background-color: var(--body-headline);
    border-top: 3px solid var(--body-headline);
    box-sizing: border-box;
    width: 45px;
    height: 3px;
    display: none;
  }
  .frameChild1 {
    position: absolute;
    background-color: var(--body-headline);
    border-top: 3px solid var(--body-headline);
    box-sizing: border-box;
    width: 91px;
    height: 3px;
    display: none;
  }
  .frameParent {
    position: absolute;
    top: 3px;
    left: 15px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
  }
  .navigationAssetTabs {
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0%;
    right: 0%;
    bottom: 0%;
    left: 0%;
  }
  .navigationAssetTabs1 {
    align-self: stretch;
    height: 31px;
    position: relative;
    display: none;
  }
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
  .createNewAssetParent {
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
  .arrowsdownIcon {
    height: 24px;
    width: 24px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .imageFrame {
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
  .parentFrame {
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
  .timespan3 {
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
  .rectangleDiv {
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
  .imageOutline1 {
    margin: 0;
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
  .chevronFrame {
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
  .frameGroup {
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
  .chevronupIcon {
    height: 20px;
    width: 20px;
    position: relative;
    object-fit: contain;
  }
  .closeAdvancedOptions {
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: center;
  }
  .loginButtonFrame {
    cursor: pointer;
    border: none;
    padding: var(--padding-base) 80px;
    background-color: transparent;
    border-top: 1px solid var(--neutral-light);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .loginButtonFrame:hover {
    background-color: rgba(105, 105, 102, 0.09);
  }
  .site1 {
    width: 58px;
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
  .site {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-9xs);
  }
  .imei {
    width: 55px;
    height: 22px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .calendarIcon {
    height: 32px;
    width: 32px;
    position: relative;
    display: none;
  }
  .timespan5 {
    align-self: stretch;
    flex: 1;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-xs) var(--padding-5xs);
  }
  .iMEITimespan {
    align-self: stretch;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-9xs);
  }
  .bleTagId {
    width: 103px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .bLETagID {
    align-self: stretch;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-xs);
    max-width: 100%;
  }
  .iMEI {
    align-self: stretch;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 4px var(--padding-12xs) var(--padding-base) 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .notes {
    width: 68px;
    height: 22px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .costcenter {
    border: 0.5px solid var(--box-stroke);
    background-color: var(--surface-background);
    height: 107px;
    width: auto;
    outline: none;
    align-self: stretch;
    border-radius: var(--br-5xs);
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xs) var(--padding-5xs);
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    color: var(--light-text);
  }
  .quantity {
    align-self: stretch;
    border-bottom: 1px solid var(--surface-dark);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base) var(--padding-base);
    gap: var(--gap-9xs);
  }
  .iMEIBLEDetails {
    align-self: stretch;
    height: 420px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    max-width: 100%;
  }
  .assetChecks {
    height: 27px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    align-items: center;
  }
  .ownershipType {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 0px var(--padding-base);
    gap: var(--gap-xl);
  }
  .timespan8 {
    align-self: stretch;
    flex: 1;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-xs);
  }
  .addAssetForm {
    align-self: stretch;
    height: 74px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-9xs);
  }
  .interval {
    width: 84px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .input {
    width: 256px;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    position: relative;
    color: var(--light-text);
    text-align: left;
    display: inline-block;
  }
  .chevronpreviousIcon {
    height: 24px;
    width: 24px;
    position: relative;
    min-height: 24px;
  }
  .timespan9 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-xs);
    gap: -4.42px;
    row-gap: 20px;
  }
  .lastMaintenance {
    width: 172px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .ddMmYyyy {
    width: 260.4px;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    position: relative;
    color: var(--light-text);
    text-align: left;
    display: inline-block;
  }
  .calendarIcon3 {
    height: 32px;
    width: 32px;
    position: relative;
  }
  .timespan10 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-5xs) var(--padding-xs);
    gap: var(--gap-xl);
  }
  .nextMaintenance {
    width: 177px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .timespan11 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-5xs);
    gap: var(--gap-xl);
  }
  .thisFieldIs3 {
    width: 156.4px;
    position: relative;
    font-size: var(--body-text-size);
    display: none;
    font-family: var(--font-open-sans);
    color: var(--status-delete);
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
  .submenu {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
    box-sizing: border-box;
    gap: var(--gap-xs);
    max-width: 100%;
  }
  .warrantyPeriod {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 16px;
    max-width: 100%;
  }
  .textFrame {
    align-self: stretch;
    border-bottom: 1px solid var(--surface-dark);
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) 0px;
    gap: var(--gap-xs);
    max-width: 100%;
  }
  .inventoryDetails {
    width: 191px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .ownershipTypeLabel {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
  }
  .assetAvailability1 {
    width: 158px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .readyToUse {
    width: 260.4px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--body-headline);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
  }
  .timespan17 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: var(--padding-xs);
    gap: var(--gap-xl);
  }
  .inventoryNumber {
    width: 166px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .quantity1 {
    width: 92px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .quantity2 {
    width: 256px;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    position: relative;
    color: var(--neutral-light);
    text-align: left;
    display: inline-block;
  }
  .chevronpreviousParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
    gap: var(--gap-mini);
  }
  .floorRoom1 {
    width: 128px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .floorRoom2 {
    width: 260.4px;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    position: relative;
    color: var(--neutral-light);
    text-align: left;
    display: inline-block;
  }
  .costCenter3 {
    width: 112px;
    height: 22px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .availabilityInfo {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-base);
    gap: var(--gap-xs);
  }
  .warrantyEnd {
    align-self: stretch;
    border-bottom: 1px solid var(--surface-dark);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) 0px;
    gap: var(--gap-xs);
  }
  .ownershipType1 {
    width: 179px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .ownershipTypeWrapper {
    align-self: stretch;
    height: 31px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .ownershipType2 {
    width: 147px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .ownershipType3 {
    width: 260.4px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    font-family: var(--noto-sans-bold-24);
    color: var(--neutral-light);
    text-align: left;
    display: inline-block;
    flex-shrink: 0;
  }
  .checkedIcon {
    height: 35px;
    width: 35px;
    position: relative;
  }
  .lowValueAsset {
    position: relative;
    font-size: var(--font-size-sm);
    font-weight: 600;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
  }
  .checkedParent {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    padding: 0px var(--padding-xl) 0px 0px;
    gap: var(--gap-xs);
  }
  .frameContainer {
    align-self: stretch;
    height: 129px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .acquisitionDate1 {
    width: 151px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .ddMmYyyy4 {
    width: calc(100% - 56px);
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    flex: 1;
    position: relative;
    color: var(--light-text);
    text-align: left;
    display: inline-block;
    min-width: 169px;
  }
  .timespan23 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-5xs) var(--padding-xs);
    gap: var(--gap-8xl);
  }
  .invoiceNumber {
    width: 146px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .costCenter5 {
    width: 100%;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    flex: 1;
    position: relative;
    color: var(--light-text);
    text-align: left;
    display: inline-block;
    min-width: 156px;
  }
  .timespan24 {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--emphasis-background);
    border: 0.5px solid var(--box-stroke);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-smi) var(--padding-xs);
  }
  .warrantyStart1 {
    width: 139px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .warrantyPeriodIn {
    width: 248px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .input1 {
    width: 256px;
    border: none;
    outline: none;
    font-family: var(--noto-sans-bold-24);
    font-size: var(--noto-sans-16-size);
    background-color: transparent;
    height: 22px;
    position: relative;
    color: var(--body-headline);
    text-align: left;
    display: inline-block;
  }
  .warrantyEnd1 {
    width: 131px;
    position: relative;
    font-size: var(--noto-sans-16-size);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--body-headline);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .assetQuantity {
    align-self: stretch;
    border-bottom: 1px solid var(--surface-dark);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-mid) var(--padding-base)
      var(--padding-base);
    gap: var(--gap-5xs);
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
    overflow-y: auto;
    flex-shrink: 0;
    display: none;
  }
  .addDocuments {
    height: 27px;
    width: 177px;
    position: relative;
    font-size: var(--font-size-xl);
    display: flex;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    align-items: center;
    padding-right: var(--padding-xl);
  }
  .addDocumentsWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .rectangle8 {
    height: 48px;
    width: 343px;
    position: relative;
    border-radius: var(--br-9xs);
    background-color: var(--surface-dark);
    display: none;
    max-width: 100%;
  }
  .imageOutline1Icon2 {
    height: 24px;
    width: 24.3px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
    z-index: 1;
  }
  .dokumentAuswhlen4 {
    position: relative;
    font-size: var(--font-size-smi);
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    z-index: 1;
  }
  .button4 {
    cursor: pointer;
    border: none;
    padding: var(--padding-smi) var(--padding-xl) var(--padding-2xs);
    background-color: var(--surface-dark);
    align-self: stretch;
    border-radius: var(--br-9xs);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    gap: var(--gap-9xs);
    max-width: 100%;
    white-space: nowrap;
  }
  .button4:hover {
    background-color: #bababa;
  }
  .img123jpg4 {
    width: 102px;
    position: relative;
    font-size: var(--body-text-size);
    display: inline-block;
    font-family: var(--font-open-sans);
    color: var(--neutral-dark);
    text-align: left;
    flex-shrink: 0;
    padding-right: var(--padding-xl);
  }
  .trashCanOutline1Icon4 {
    height: 16px;
    width: 16.2px;
    position: absolute;
    margin: 0 !important;
    right: 12.1px;
    bottom: -2px;
    overflow: hidden;
    flex-shrink: 0;
  }
  .trashCan {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    position: relative;
  }
  .frameSection {
    align-self: stretch;
    border-bottom: 1px solid var(--surface-dark);
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-base) var(--padding-mid) 18px var(--padding-base);
    gap: var(--gap-xs);
    max-width: 100%;
  }
  .saveAsset {
    margin: 0;
    height: 33px;
    position: relative;
    font-size: var(--noto-sans-bold-24-size);
    font-weight: 700;
    font-family: var(--noto-sans-bold-24);
    color: var(--surface-white);
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .pillLoginLong {
    flex: 1;
    border-radius: var(--br-50xl);
    background-color: var(--toolsense-bold-links);
    box-shadow: var(--primary-button-shadow);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-2xs);
    box-sizing: border-box;
    max-width: 100%;
    white-space: nowrap;
  }
  .loginButton {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-smi) var(--padding-mid) var(--padding-mid) 14px;
    box-sizing: border-box;
    opacity: 0.5;
    max-width: 100%;
    cursor: pointer;
  }
  .blankQrAddAssetQuickF {
    margin: 0;
    width: 376px;
    background-color: var(--surface-white);
    box-shadow: var(--dropshadow-board);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    letter-spacing: normal;
  }
</style>
