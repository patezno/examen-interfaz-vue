<template>
    <div id="Card">
          <div v-for="player in players" :key="player.title" class="row">
            <div class="col s12 m7">
                <div class="card">
                    <div class="card-image">
                        <img v-bind:src="player.src">
                        <span class="card-title">{{player.title}}</span>
                    </div>
                    <div class="card-content">
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

</style>