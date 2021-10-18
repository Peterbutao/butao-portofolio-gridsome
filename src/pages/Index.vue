<template>
  <Layout>
    <SectionOne />
    <SectionTwo v-bind:projects="projects"/>
    <SectionThree v-bind:about="about"/>
    <SectionFour />
  </Layout>
</template>

<script>
import SectionOne from "../components/SectionOne.vue"
import SectionTwo from "../components/SectionTwo.vue"
import SectionThree from "../components/SectionThree.vue"
import SectionFour from "../components/SectionFour.vue"
export default {
  metaInfo: {
    title: 'Home | '
  },
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour
  },
  data() {
    return{
      projects:[
        {
          name: "ZIDA NATION",
          logo: "/logo1",
          meta: "Zida Nation Malawi, Apremium lifestyle music group. Supporting and producing local urban malawian trends. "
        },
        {
          name: "LUANAR BSSY TIMETABLE",
          logo: "/logo2",
          meta: " LUANAR student daily timetable, Dynamic data reflecting student classes. Hybrid Application built on cordova"
        },
        {
          name: "MAKA ANIMATION STUDIOS",
          logo: "/logo3",
          meta: " Founded in 2017, aims to produce malawian based stories , through animations and art. "
        }
      ],
      about: [
        {
          id: "f4f4h",
          paragraph: "Highly passionate and successful UI/UX designiner, with experience in visual UI design , usability interaction design , hyper text markup language , Javasrcipt and Js frameworks , Css , usability interaction design , python automation language , [machine learning, web applications, task automation]. Recognized as a talented problem solver with a unique skill set, spaning in multiple disciplines"
        }
      ]

    }
  }
}
</script>


