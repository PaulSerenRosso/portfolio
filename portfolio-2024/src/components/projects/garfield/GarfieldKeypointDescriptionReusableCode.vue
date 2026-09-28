<script>
import {defineComponent} from 'vue'
import SpaceParagraph from "@/components/SpaceParagraph.vue";
import MainParagraph from "@/components/MainParagraph.vue";
import BoldElement from "@/components/BoldElement.vue";
import LinkElement from "@/components/LinkElement.vue";

export default defineComponent({
  name: "GarfieldKeypointDescriptionReusableCode",
  components: {LinkElement, BoldElement, MainParagraph, SpaceParagraph}
})
</script>

<template>
  <space-paragraph>
    At OSome, we follow the principle that, whenever we create code, we decide which codebase it belongs in: the
    <bold-element> Garfield-specific codebase</bold-element> or the  <bold-element>codebase shared by all games</bold-element>. I contributed to this approach and
    strongly advocated for it.
    For example, I took several <bold-element>existing features during the production</bold-element>, such as the <bold-element>dialogue/cutscene</bold-element> systems and
    the <bold-element>save system</bold-element>, which were initially developed mainly in the Garfield codebase, and progressively I extracted parts
    of them so they could be reused in the OSome codebase.
  </space-paragraph>
  <space-paragraph> <bold-element> I created most of the UI for Garfield</bold-element>, and following this logic was also responsible for <bold-element>isolating a UI framework</bold-element> that
    could be <bold-element>reused in future games</bold-element>.
  I created custom versions of <bold-element>UI components</bold-element>, such as buttons and sliders, to improve <bold-element>focus handling</bold-element>
    and <bold-element>visual feedback</bold-element>.  I also developed more complex components, including a <bold-element>carousel</bold-element>, a  <bold-element>warning-save widget</bold-element>, timers, and
    counters.  </space-paragraph>

  <space-paragraph>Through discussions with our <bold-element>lead game designer</bold-element>, I also implemented various systems to maintain
    <bold-element>interface consistency</bold-element>. For example, I created a <bold-element>padding handler</bold-element> that allowed us to apply custom padding to an
    element using a predefined list, similar to <link-element  link="https://developer.mozilla.org/en-US/docs/Web/CSS">CSS styles</link-element>.
    I applied the same principle to text by creating a custom version of the <link-element link="https://dev.epicgames.com/documentation/unreal-engine/umg-rich-text-blocks-in-unreal-engine?lang=en-US">Rich Text Block</link-element>. It included
    specific behaviors, such as allowing tags within the text to create line breaks or insert input icons. Together with the <bold-element>game and narrative designers</bold-element>, I was responsible for ensuring that <bold-element>localization</bold-element> was
    correctly integrated into the UI framework.

  </space-paragraph>
  <main-paragraph>After that, I added more <bold-element>advanced features</bold-element> to the framework, such as  <bold-element>loading screens</bold-element>,  <bold-element>pop-ups</bold-element>,
    <bold-element> credits</bold-element>,  <bold-element>fade effects</bold-element>,  <bold-element>the main menu</bold-element>,  <bold-element>the pause menu</bold-element>, and  <bold-element>startup screens </bold-element> systems.
    Moreover, I created the <bold-element>options system</bold-element>. This was particularly useful because it allowed <bold-element>other
      programmers</bold-element> to <bold-element> add new options easily</bold-element> across the save system, the options menu, and the different managers.
  </main-paragraph>
</template>

<style scoped lang="scss">

</style>
