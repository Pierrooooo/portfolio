<template>
  <section class="skills_container">
      <h2>Skills</h2>
    <div class="skills">
      <div class="skill" v-for="skill in skills" v-bind:key="skill.skillName" style="background-image: url('skill.imgPath')" >
        <h3>{{skill.skillName}}</h3>
        <p>{{skill.desc}}</p>
      </div>
    </div>
  </section>
</template>

<script>
import imgPathUXUI from '~/assets/imgs/icons/skills/UXUI.jpg'
export default {
  name: 'Skills',
  data () {
    return {
      skills:[
        {
          skillName:'UX/UI',
          desc:'I like to try what\'s more user friendly. And I also like to make things great looking.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/UXUI.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'Figma',
          desc:'I use figma to make wireframes/models and I\'m learning to animate and prototyping them.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/Figma.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'XD',
          desc:'I also use XD as I use Figma it depends on the team needs.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/XD.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'Creative Cloud',
          desc:'I like to do some artistic personal projects on Photoshop, Illustrator or After Effects.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/creativecloud.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'Javascript',
          desc:'I mostly made API calls, injecting HTML & changing style to HTML elements. I really enjoyed working with this language.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/JS.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'HTML',
          desc:'It\'s the first thing i started to learn with CSS.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/HTML.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'CSS',
          desc:'I now use SCSS which is a superset of CSS and make it easier to read and navigate into your files.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/CSS.jpg\');',
          imgPath: imgPathUXUI,
        },
        {
          skillName:'Wordpress',
          desc:'I do Wordpress with the plugin Advanced Custom Fields beacause it make the back office simple to setup. And I can change the content at any time very easily.',
          image: 'background-image: url(\'~/assets/imgs/icons/skills/Wordpress.jpg\');',
          imgPath: imgPathUXUI,
        },
      ]
    }
  }
}
</script>

