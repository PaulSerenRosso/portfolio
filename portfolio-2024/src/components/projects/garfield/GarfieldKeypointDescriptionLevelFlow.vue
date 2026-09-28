<script>
import {defineComponent} from 'vue'
import SpaceParagraph from "@/components/SpaceParagraph.vue";
import MainParagraph from "@/components/MainParagraph.vue";
import BoldElement from "@/components/BoldElement.vue";
import LinkElement from "@/components/LinkElement.vue";

export default defineComponent({
  name: "GarfieldKeypointDescriptionLevelFlow",
  components: {LinkElement, BoldElement, MainParagraph, SpaceParagraph}
})
</script>

<template>
  <space-paragraph>Because much of the UI I created was designed to visually represent the <bold-element>player's progression</bold-element>, I often developed those level-flow systems.
 This included for example, the standard mode, the <bold-element>Foodometer</bold-element>, whose objective was to collect enough lasagnas and
    snacks or find special lasagnas throughout the level. I was also responsible for developing an alternate mode called
    <bold-element>Time Attack</bold-element>, in which the goal was to complete the level within a specific time limit.
  </space-paragraph>
  <space-paragraph>Some levels had specific flows, such as <bold-element>wave systems</bold-element> with objectives like defeating all enemies or
    collecting snacks. I created the UI for these systems while also improving and fixing the existing code. I <bold-element>reused
      parts</bold-element> of this system for levels featuring ribs and eggplants, which Garfield could mount to reach specific
    destinations. Throughout production, I balanced <bold-element>code quality, maintainability, and deadline requirements</bold-element>. In some
    cases, such as this last, using a <bold-element>focused workaround</bold-element> was more appropriate than creating perfectly clean code for a
    feature limited to a small number of levels.
  </space-paragraph>
  <space-paragraph>For meta-progression, I took responsibility for the <bold-element>Jon's House</bold-element> after several programmers and designers
    had already worked on it. I fixed issues in the Jon'House, added the HUD for the <bold-element>unlocking sequence</bold-element>,
    and improved how completed layouts were saved.
  </space-paragraph>

  <main-paragraph>I created a   <bold-element>metadata system</bold-element> for our <bold-element>levels</bold-element>. It contained <bold-element>static informations</bold-element> about the current level,
    such as the number of lasagnas, the level name, and its biome data. This system was particularly useful when I
    developed the <bold-element>Overworld HUD</bold-element> and the <bold-element>Quick Select menu</bold-element>, which allowed players to teleport to a specific level node on
    the map. I also worked on a <bold-element>generic announcement</bold-element> system and was responsible for the <bold-element>tutorial</bold-element> system. Finally, I
    helped programmers iterate on the new level-scripting system for future projects, based on an <bold-element>actor input/output</bold-element>
    system similar to the one used in the <link-element link="https://developer.valvesoftware.com/wiki/Source">Source engine</link-element>.
  </main-paragraph>
</template>

<style scoped lang="scss">

</style>
