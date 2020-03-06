<template>
    <div id="Card">
          <div class="row">
            <div v-for="(player, index) in players" :key="player.title" class="col s12 m6 l3">
                <div class="card">
                    <div class="card-image">
                        <img class="photo" v-if="player.src" :src="player.src" alt="photo">
                        <img class="photo" v-else src="../assets/images/no-image.jpg" alt="no-image">
                        <span class="card-title">{{player.title}}</span>
                    </div>
                    <div class="card-content card-large" v-bind:class="{'grey-card': index % 2 !== 0 }">
                        <p>{{player.text}}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['players']
}
</script>

<style lang="scss" scoped>

.card-large {
    height: 260px; 
}

.grey-card {
    background: grey;
}

</style>