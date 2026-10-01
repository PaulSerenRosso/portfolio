<script>
import {defineComponent} from 'vue'
import SpaceParagraph from "@/components/SpaceParagraph.vue";
import MainParagraph from "@/components/MainParagraph.vue";
import LinkElement from "@/components/LinkElement.vue";
import BoldElement from "@/components/BoldElement.vue";

export default defineComponent({
  name: "GarfieldKeypointDescriptionUiFramework",
  components: {BoldElement, LinkElement, MainParagraph, SpaceParagraph}
})
</script>

<template>
  <space-paragraph>At the <bold-element>beginning of the project</bold-element>, we needed an initial version of the UI before there was enough time
    to complete the framework’s R&D. I therefore <bold-element>prototyped the initial UI</bold-element> so that the team could start working with it
    immediately. I then tested <bold-element>different approaches</bold-element> to creating <bold-element> UI</bold-element> in Unreal Engine. I <bold-element>documented</bold-element> my  <bold-element>benchmarks</bold-element> and  <bold-element>presented</bold-element> the results during our weekly  <bold-element>Tech Review meetings</bold-element>, where
    programmers shared progress, discussed challenges, and coordinated with QA and technical game designers.
    We ultimately chose
    <link-element
      link="https://dev.epicgames.com/documentation/unreal-engine/common-ui-plugin-for-advanced-user-interfaces-in-unreal-engine?lang=en-US">
      Common UI
    </link-element>
     with <link-element link="https://dev.epicgames.com/documentation/unreal-engine/umg-ui-designer-quick-start-guide-in-unreal-engine?lang=en-US">UMG</link-element> , as used in <link-element link="https://www.playrematch.com/">Rematch</link-element> and <link-element link="https://www.fortnite.com/">Fortnite</link-element>, supported by a layer of <bold-element>custom code</bold-element> designed to meet our
    <bold-element>specific needs</bold-element>.
  </space-paragraph>
  <space-paragraph>During <bold-element>production</bold-element>, I encountered several <bold-element>limitations in Common UI</bold-element>. Although Common UI helped us deliver
    the UI quickly at the beginning of the project, some <bold-element>edge cases</bold-element> were not handled, and certain <bold-element>features did not work</bold-element>
    as expected. Rewriting it from scratch was not a realistic option. Instead, I focused on <bold-element>fixing</bold-element> and <bold-element>improving</bold-element> key
    systems, including the <bold-element>menu stack</bold-element> and <bold-element>input interactions</bold-element>. Over time, the custom-code layer expanded to support cases
    that Common UI could not handle on its own.
  </space-paragraph>
  <space-paragraph>At the <bold-element>end of the project</bold-element>, I <bold-element>reviewed</bold-element> the <bold-element>framework’s architecture</bold-element>. As I was the main programmer using it
    on Garfield, I wanted to make it easier for other programmers to implement UI while maintaining consistency across
    systems. I <bold-element>documented</bold-element> several  <bold-element>patterns</bold-element> to make UI implementation more <bold-element>accessible</bold-element> and <bold-element>consistent</bold-element>.
  </space-paragraph>

  <main-paragraph>For our <bold-element>menus</bold-element>, I established a <bold-element> ViewModel</bold-element> pattern. For <bold-element>smaller UI</bold-element> elements, I promoted <bold-element>simple, focused
    implementations</bold-element>. In <bold-element>complex HUDs</bold-element>, I encouraged grouping related data into <bold-element>structs</bold-element>. I also established a clear
    separation of responsibilities: <bold-element>UI logic and UI Component binding declarations</bold-element> should be handled in <bold-element>C++</bold-element>, while the <bold-element>binding implementations</bold-element> and <bold-element>Ui layout</bold-element> should
    remain in <bold-element>Blueprints</bold-element>. This approach also makes it possible to create <bold-element>multiple layouts</bold-element> that share the <bold-element>same underlying behavior</bold-element>. Finally, I structured the <bold-element>data flow</bold-element> so that <bold-element>dedicated systems</bold-element> receive <bold-element>gameplay data</bold-element>, process and
    <bold-element>convert </bold-element>it for the UI, and <bold-element>send</bold-element> properly formatted data to the  <bold-element>UI layer</bold-element>.
  </main-paragraph>
</template>

<style scoped lang="scss">

</style>
