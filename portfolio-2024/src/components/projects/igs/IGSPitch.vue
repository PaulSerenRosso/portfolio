<script>
import {defineComponent} from 'vue'
import SpaceParagraph from '@/components/SpaceParagraph.vue'
import MainParagraph from '@/components/MainParagraph.vue'
import LinkElement from "@/components/LinkElement.vue";
import BoldElement from "@/components/BoldElement.vue";

export default defineComponent({
  name: 'IGSPitch',
  components: {BoldElement, MainParagraph, SpaceParagraph},
})
</script>

<template>
  <div>
    <space-paragraph>
      The idea behind this personal project is simple: each prototype
      is like a <bold-element>solo game jam</bold-element>, except the theme is inspired by a <bold-element>real-world issue</bold-element>.
    </space-paragraph>
    <space-paragraph>
      The time limit challenges me to <bold-element>quickly design</bold-element> a playable prototype that tests whether a
      gameplay concept is <bold-element>fun</bold-element>. Each project is also an opportunity to <bold-element>experiment</bold-element>
      with <bold-element>new technologies</bold-element>, game engines, genres, and mechanics that I haven't worked with before.
    </space-paragraph>
      <space-paragraph>
        I chose to develop these prototypes entirely on my own so I could <bold-element>learn skills beyond programming</bold-element>, including game
      design, art, audio, and other disciplines involved in game development.
      </space-paragraph>
    <space-paragraph>
      My goal is not only to create enjoyable prototypes but also to <bold-element>learn how to raise awareness</bold-element> through video games about important real-world issues.
      That's why each prototype explores a <bold-element>different theme</bold-element>, allowing me to experiment with new subjects!
      </space-paragraph>
    <main-paragraph>
      Below, you'll find a summary of each prototype.
    </main-paragraph>



  </div>
</template>

<style scoped lang="scss"></style>
