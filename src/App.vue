<template>
  <div id="app">
    <Navbar></Navbar>
    <Card :players="players"></Card>
    <Footer></Footer>
  </div>
</template>

<script>
import Card from './components/Card';
import Navbar from './components/Navbar';
import Footer from './components/Footer';

export default {
  name: 'App',
  components: {
    Card,
    Navbar,
    Footer
  },
  data: () => ({
    players: [
            {
                title: "Judit Polgar",
                text: "Judit Polgar is widely regarded as the strongest female chess player of all time. She achieved a peak rating of 2735 and earned the title of Grandmaster in 1991. At the height of her career, Polgar made her way onto several top 10 lists of best active chess players � male or female",
                src: require("@/assets/images/juditpolgar.jpg")
            },
            {
                title: "Susan Polgar",
                text: "Susan Polgar is the older sister of Judit Polgar, and one of chess�s most famous female players. Like her sisters, she was a chess prodigy and later went on to achieve many prestigious titles. For example, Susan Polgar was the first woman to earn the title of Grandmaster",
                src: require("@/assets/images/susanpolgar.jpg")
            },
            {
                title: "Anna Rudolf",
                text: "Rudolf spent her childhood in B�tasz�k, a small town in southern Hungary. She started to play chess along with her sister Kata at the age of four. Many competitions and successes followed. From a young age she maintained a position as one of Hungary's top players",
                src: ""
            },
            {
                title: "Maya Chiburdanidze",
                text: "Maya (also spelled Maia) Chiburdanidze is a Georgian grandmaster, and the only chess player in history to have won nine Chess Olympiads. In 1978, she won the Women�s World Chess Championship by defeating the reigning champion",
                src: require("@/assets/images/maya.jpg")
            },
            {
                title: "Anna Muzychuk",
                text: "Muzychuk was taught to play chess at the age of two by her parents, both professional chess coaches. She played her first tournament at five and in the same year she placed second in the under-10 girls championship of Lviv Oblast.",
                src: ""
            },
            {
                title: "Rohini Khadilkar",
                text: "Rohini Khadilkar is the youngest of the famous Khadilkar sisters. She won the Indian Women�s Chess Championship 5 times and went on to compete in the 1976 Indian Men�s Chess Championship.",
                src: require("@/assets/images/rohini.jpg")
            },
            {
                title: "Xie Jun",
                text: "Xie Jun is the Chinese chess player who ended Maya Chiburdanidze�s 14 year long reign in 1991. She was the star that signalled China�s ascent into dominance in the field of women�s chess.",
                src: require("@/assets/images/xiejun.jpg")
            },
            {
                title: "Vera Menchik",
                text: "Vera Menchik is the original Women�s World Chess Champion, and the longest reigning champion to date. She dominated the first WWCC in 1927, and continued to do so in each of the 6 consecutive championships",
                src: require("@/assets/images/vera.jpg")
            },
            {
                title: "Ana Matnazde",
                text: "She is a Georgian-Spanish chess player. FIDE awarded her the titles Woman Grandmaster (WGM), in 2002, and International Master (IM), in 2006. Matnadze was European and world girls champion in her age category.",
                src: ""
            }
        ]
  })
}
</script>

<style lang="scss">
$font: Helvetica;
$color: #334166;
html {
  width: 75%;
  margin: 0 auto;
  font-family: $font
}

@media (max-width: 600px) {
    html {
      width: 100%;
    }
}
</style>
