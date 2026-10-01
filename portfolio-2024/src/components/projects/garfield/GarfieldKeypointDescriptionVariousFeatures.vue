<script>
import {defineComponent} from 'vue'
import SpaceParagraph from "@/components/SpaceParagraph.vue";
import MainParagraph from "@/components/MainParagraph.vue";
import BoldElement from "@/components/BoldElement.vue";
import LinkElement from "@/components/LinkElement.vue";

export default defineComponent({
  name: "GarfieldKeypointDescriptionVariousFeatures",
  components: {LinkElement, BoldElement, MainParagraph, SpaceParagraph}
})
</script>

<template>
  <space-paragraph>When a programmer’s
    workload became too heavy, I provided support by taking on <bold-element>individual tasks</bold-element> or, when necessary, taking <bold-element>full
      ownership</bold-element> of a <bold-element>new/existing feature</bold-element> to help reduce their workload over the long term.
  </space-paragraph>
  <space-paragraph>I worked on the <bold-element>3Cs</bold-element>  and created Garfield’s
    <bold-element>attack combo system</bold-element> linked to the <bold-element>input-buffering</bold-element> and abilities like the <bold-element>gain</bold-element> of <bold-element>costume</bold-element> or of <bold-element>lasagna</bold-element> and I contributed to the <bold-element>lasso cowboy</bold-element> and <bold-element>crocodile</bold-element> features. We have integrated <link-element link="https://dev.epicgames.com/documentation/unreal-engine/gameplay-ability-system-for-unreal-engine?lang=en-US">GAS</link-element> (the Gameplay Ability System), because it gave a <bold-element>great structure</bold-element> for our codebase particularly useful!
    </space-paragraph>
  <space-paragraph>
    I also
    <bold-element>refactored prototype code</bold-element>
    such as
    <bold-element>collectible/chest</bold-element>
    systems, the activation system for level design elements created by the
    <bold-element>technical game designers</bold-element>.
    It was challenging because these feature prototypes were already <bold-element>linked to multiple levels</bold-element> and assets. The goal was to
    refactor without <bold-element>breaking too many references</bold-element> or forcing <bold-element> level designers to rebuild their setups</bold-element>. To achieve
    this, I provided <bold-element>guidelines</bold-element> for the technical game designers  to make code refactoring easier. I documented and use some techniques including <link-element link="https://dev.epicgames.com/documentation/unreal-engine/editor-utility-widgets-in-unreal-engine">Editor Utility Widgets</link-element>
    including <link-element link="https://dev.epicgames.com/documentation/unreal-engine/core-redirects-in-unreal-engine?lang=en-US">Core Redirects</link-element>, <bold-element>reparenting</bold-element>, and <bold-element>resaving assets command</bold-element>.
  </space-paragraph>
  <space-paragraph>
    I also completely refactored the <bold-element>projectile </bold-element>system
    and <bold-element>projection abilities</bold-element> and created a <bold-element>pattern</bold-element> system. These systems had initially been prototyped quickly and
    required a more robust structure to support the rest of production.
    They were used for <bold-element>enemies</bold-element>, <bold-element>bosses</bold-element>, and certain level design elements, such as the <bold-element>cannon</bold-element>.
    The goal of the projectile system was to make it <bold-element>easily adjustable</bold-element> by the <bold-element>game designers</bold-element> from a
    <bold-element>central location</bold-element>. It also allowed technical game designers to  <bold-element>create patterns themselves</bold-element>.
  </space-paragraph>

  <main-paragraph>
    I also supported  <bold-element>AI programming</bold-element> for example by working on <bold-element>shooter enemies</bold-element>, the skewer enemy, which is composed of several smaller
    enemies, as well as the eggplant and rib enemies and the <bold-element>rodeo system</bold-element> that allows Garfield to mount them.
    Working on the gameplay features of a 3D platformer was particularly interesting to me because they needed to feel <bold-element>juicy, responsive, and satisfying</bold-element>. It was also rewarding to exchange ideas
    with <bold-element>animators</bold-element> and <bold-element>designers</bold-element> to determine the best ways to improve the experience and decide which areas to
    <bold-element> prioritize</bold-element> within the available time.
  </main-paragraph>
</template>

<style scoped lang="scss">

</style>
