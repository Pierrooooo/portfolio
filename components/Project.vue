<template>
  <div class="projects">
    <div class="project" v-for="project in projects" v-bind:key="project.projectName" >
      <p class="count " data-count="" v-if="count<10">0{{count++}}</p>
      <p class="count" v-else>{{count++}}</p>

      <!-- <img :srcset="backgrounds[randomNumber()]"> -->
      <img src="~assets/imgs/Meteor.svg" alt=""><!--  img du projet -->
      <div>
        <h3>{{project.projectName}}</h3>
        <p><span v-for="tech in project.techs" v-bind:key="tech"> {{tech}}</span></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data () {
    return {
      count: -403,
      projects:[
        {
          projectName:'Space Travelor',
          projectCount: '01',
          techs:[
            'HTML',
            'CSS',
            'Javascript',
          ],
          imgProjectPath:'~assets/imgs/SoundWave.svg',
          who:'Just me',
          desc:'This is an individual class projet in witch I had to use at minimu 2 API. I decided to do something that would be pretty unique so I decided to make a selector in the principal theme of StarWars. I couldn\'t use the PokemonApi because we already used it in a previous class. I searched API with characters that i like and that everyone know the existence. When I had the idea of my site and the differents API I wanted to use, the \'only\' things to do left was coding. It took me some time to achive the objectives what I `\'ve fixed to myself and it\'s not finished yet. I still have to factorise my Api calls with some dataset attribute and to fixed little things in css.',
          link:'https://space-travelor.8pier.re/',
          github:'https://github.com/Pierrooooo/api_Travel_Space',
        },
        {
          projectName:'First Portfolio',
          projectCount: '02',
          techs:[
            'HTML',
            'Sass',
            'Javascript',
          ],
          imgProjectPath:'~assets/imgs/SoundWave.svg',
          who:'Just me',
          desc:'This is an individual projet, it\'s also my first portfolio, I\'ve done it in one week on november 2021. We had to do all the designs and coding by our own and I wanted to do a site with colors i enjoyed at this time, pastel\'s one. I think it was a little bit to ambicious for the experience I had in Web Design. ',
          link:'https://portfolio-a2-theta.vercel.app/',
          github:'https://github.com/Pierrooooo/Portfolio_A2',
        },
        {
          projectName:'Second Portfolio',
          projectCount: '03',
          techs:[
            'HTML',
            'Sass',
            'Javascript',
          ],
          imgProjectPath:'~assets/imgs/SoundWave.svg',
          who:'Just me',
          desc:'This project is a class projet, it\'s also my second portfolio, I\'ve mostly done it on my chrismas holidays. We had to do all the designs and coding by our own and I wanted to do a dark theme with the red/pink color that I love 😍!!',
          link:'https://8pier.re',
          github:'https://github.com/Pierrooooo/PortfolioV2',
        },
        {
          projectName:'BAP Medi-Link',
          projectCount: '04',
          techs:[
            'Wordpress',
            'PHP',
            'Sass',
            'Javascript',
          ],
          imgProjectPath:'~assets/imgs/SoundWave.svg',
          who:'Group Project',
          desc:'This is a BAP(Bourse Aux Projects = project stock exchange) project,The client needed a new website to show what his company work\'s concist.We decided to go on a Mobile first vision because he told us that we wanted to put a QR code on a banner he would show on trade fair. I worked on the zoning, Wordpress setup & backoffice data creation and front integration.',
          link:'',
          github:'https://github.com/BAP44/medilink',
        },
      ],
      backgrounds:[
        '~assets/imgs/SoundWave.svg',
        "\"data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' version='1.1' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:svgjs='http://svgjs.com/svgjs' width='960' height='540' preserveAspectRatio='none' viewBox='0 0 960 540'%3e%3cg mask='url(%26quot%3b%23SvgjsMask1214%26quot%3b)' fill='none'%3e%3crect width='960' height='540' x='0' y='0' fill='rgba(6%2c 15%2c 34%2c 1)'%3e%3c/rect%3e%3cpath d='M573 204L936 -159' stroke-width='8' stroke='url(%23SvgjsLinearGradient1215)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M160 214L533 -159' stroke-width='6' stroke='url(%23SvgjsLinearGradient1216)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M246 504L466 284' stroke-width='10' stroke='url(%23SvgjsLinearGradient1217)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M436 33L811 -342' stroke-width='10' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M673 6L388 291' stroke-width='8' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M131 503L331 303' stroke-width='10' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M499 144L275 368' stroke-width='8' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M676 329L503 502' stroke-width='10' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M436 477L197 716' stroke-width='6' stroke='url(%23SvgjsLinearGradient1217)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M434 523L297 660' stroke-width='6' stroke='url(%23SvgjsLinearGradient1215)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M247 245L-83 575' stroke-width='6' stroke='url(%23SvgjsLinearGradient1219)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M392 124L713 -197' stroke-width='8' stroke='url(%23SvgjsLinearGradient1219)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M218 475L477 216' stroke-width='8' stroke='url(%23SvgjsLinearGradient1216)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M274 241L620 -105' stroke-width='10' stroke='url(%23SvgjsLinearGradient1217)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M716 227L488 455' stroke-width='6' stroke='url(%23SvgjsLinearGradient1215)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M798 447L661 584' stroke-width='8' stroke='url(%23SvgjsLinearGradient1219)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M858 252L560 550' stroke-width='6' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M577 237L411 403' stroke-width='10' stroke='url(%23SvgjsLinearGradient1215)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M524 371L677 218' stroke-width='8' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M871 231L1222 -120' stroke-width='10' stroke='url(%23SvgjsLinearGradient1215)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M815 474L460 829' stroke-width='10' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M473 119L250 342' stroke-width='10' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M551 93L805 -161' stroke-width='8' stroke='url(%23SvgjsLinearGradient1218)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M622 155L967 -190' stroke-width='6' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3cpath d='M7 325L-169 501' stroke-width='10' stroke='url(%23SvgjsLinearGradient1219)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M268 281L544 5' stroke-width='10' stroke='url(%23SvgjsLinearGradient1216)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M159 488L492 155' stroke-width='6' stroke='url(%23SvgjsLinearGradient1219)' stroke-linecap='round' class='TopRight'%3e%3c/path%3e%3cpath d='M10 353L159 204' stroke-width='10' stroke='url(%23SvgjsLinearGradient1220)' stroke-linecap='round' class='BottomLeft'%3e%3c/path%3e%3c/g%3e%3cdefs%3e%3cmask id='SvgjsMask1214'%3e%3crect width='960' height='540' fill='white'%3e%3c/rect%3e%3c/mask%3e%3clinearGradient x1='0%25' y1='100%25' x2='100%25' y2='0%25' id='SvgjsLinearGradient1215'%3e%3cstop stop-color='rgba(38%2c 88%2c 205%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(38%2c 88%2c 205%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3clinearGradient x1='0%25' y1='100%25' x2='100%25' y2='0%25' id='SvgjsLinearGradient1216'%3e%3cstop stop-color='rgba(205%2c 38%2c 88%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(205%2c 38%2c 88%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3clinearGradient x1='100%25' y1='0%25' x2='0%25' y2='100%25' id='SvgjsLinearGradient1217'%3e%3cstop stop-color='rgba(205%2c 38%2c 88%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(205%2c 38%2c 88%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3clinearGradient x1='100%25' y1='0%25' x2='0%25' y2='100%25' id='SvgjsLinearGradient1218'%3e%3cstop stop-color='rgba(38%2c 88%2c 205%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(38%2c 88%2c 205%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3clinearGradient x1='0%25' y1='100%25' x2='100%25' y2='0%25' id='SvgjsLinearGradient1219'%3e%3cstop stop-color='rgba(60%2c 211%2c 175%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(60%2c 211%2c 175%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3clinearGradient x1='100%25' y1='0%25' x2='0%25' y2='100%25' id='SvgjsLinearGradient1220'%3e%3cstop stop-color='rgba(60%2c 211%2c 175%2c 0)' offset='0'%3e%3c/stop%3e%3cstop stop-color='rgba(60%2c 211%2c 175%2c 1)' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3c/defs%3e%3c/svg%3e\"",
        '~assets/imgs/Sprinkle.svg',
      ],
    }
  },
    methods : {
    randomNumber : function(){
      return Math.floor(Math.random() * (this.backgrounds.length - 0 + 1));
    }
  }
}
</script>
