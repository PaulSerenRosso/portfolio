<script>
import {defineComponent} from 'vue'
import SpaceParagraph from "@/components/SpaceParagraph.vue";
import MainParagraph from "@/components/MainParagraph.vue";
import BoldElement from "@/components/BoldElement.vue";

export default defineComponent({
  name: "GarfieldKeypointDescriptionPlatform",
  components: {BoldElement, MainParagraph, SpaceParagraph}
})
</script>

<template>
  <space-paragraph>I cannot discuss the development of Garfield without mentioning its development for both PC and
    consoles. This introduced a wide range of constraints and challenges that I needed to handle.
  </space-paragraph>
  <space-paragraph>For the UI, I made the pause menu adapt its <bold-element>control scheme</bold-element> according to the platform and connected
    gamepad . Throughout the UI, <bold-element>input icons</bold-element> also changed based on the platform and gamepad being used.
    <bold-element>Navigation</bold-element> needed to work seamlessly with a  gamepad, keyboard, and mouse, especially in
    menus containing <bold-element>multiple stacks</bold-element>. The  <bold-element>focus</bold-element> always needed to be correctly managed.
    I also handled the <bold-element>pop-up system</bold-element>, which needed to be robust and simple to use to support <bold-element>console-specific
      alerts</bold-element>, such as gamepad disconnections. And the <bold-element>list of the options</bold-element> needed to be platform specific.
  </space-paragraph>
  <space-paragraph>Garfield needed to support both <bold-element>French AZERTY and QWERTY keyboards</bold-element>. The game also needed to support
    the inversion of the <bold-element>A and B buttons</bold-element> on Nintendo Switch controllers compared with traditional gamepads. In both
    cases, I ensured that the UI displayed the correct inputs and that gameplay and UI input mappings were configured
    correctly.
  </space-paragraph>
  <main-paragraph>I also helped debug and test the <bold-element>game’s performance on Nintendo Switch</bold-element>. I resolved <bold-element>GPU- and
    CPU-specific issues</bold-element>, as well as problems that were specific to particular <bold-element>levels</bold-element> or <bold-element>global systems</bold-element>.
    Finally, <bold-element>console save data</bold-element> was managed on a <bold-element>per-user
      basis</bold-element>. I therefore needed to ensure that saves were correctly handled for each user, even when multiple users were
    playing on the same console.
  </main-paragraph>
</template>

<style scoped lang="scss">

</style>
