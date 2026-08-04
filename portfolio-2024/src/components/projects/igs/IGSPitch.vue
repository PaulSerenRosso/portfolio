<script>
import {defineComponent} from 'vue'
import SpaceParagraph from '@/components/SpaceParagraph.vue'
import MainParagraph from '@/components/MainParagraph.vue'
import LinkElement from "@/components/LinkElement.vue";
import BoldElement from "@/components/BoldElement.vue";

export default defineComponent({
  name: 'IGSPitch',
  components: {BoldElement, LinkElement, MainParagraph, SpaceParagraph},
})
</script>

<template>
  <div>
    <space-paragraph>
      <link-element link="https://www.osome-studio.com/">OSome Studio</link-element>
      develops games for PC and consoles, including licensed franchises. The company has released
      <bold-element>family-oriented</bold-element> games based on popular European IPs like <bold-element>Asterix and Obelix</bold-element> or <bold-element>The Smurfs</bold-element>.
    </space-paragraph>
    <space-paragraph>
      <link-element link="https://store.steampowered.com/app/3932790/Garfield__Escape_from_Monday/"> Garfield Escape
        From Monday</link-element>
      is an upcoming <bold-element>3D platformer</bold-element> published by
      <link-element link="https://www.microids.com/">Microids</link-element>.
     Here's a small pitch:
    </space-paragraph>
      <main-paragraph>"After Jon makes Garfield eat spinach lasagna recommended by Chef Monday, he falls into a deep sleep and becomes
        <bold-element>trapped</bold-element> in a <bold-element>bizarre dream</bold-element> world ruled by Monday itself. The world’s laziest cat must navigate through
        <bold-element>enemy-filled</bold-element> levels, collect as many lasagnas as possible, and fight his way toward <bold-element>waking up</bold-element> and <bold-element>regaining his
          sense of taste</bold-element>. Gameplay focuses on <bold-element>fluid feline movement</bold-element> such as jumping, rolling into a ball, and climbing
        walls, always landing on his feet. Along the way, Garfield can rely on Jon and his friends Odie, Arlene, and
        Pookie, while enemies like Nermal and Squeak try to stop him. He can also unlock <bold-element>hilarious costumes</bold-element> like a turkey,
        surfer, or cowboy, each <bold-element>granting unique abilities</bold-element>. Across <bold-element>three vibrant worlds</bold-element> and dozens of levels, players
        <bold-element>collect lasagna</bold-element> and other items that not only help progression but also allow them to <bold-element>decorate Jon’s house</bold-element>."
    </main-paragraph>
  </div>
</template>

<style scoped lang="scss"></style>
