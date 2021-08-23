<template>
    <div>
        <img src="https://www.awn.com/sites/default/files/styles/original/public/image/featured/1046202-sympathy-devil-how-digital-domain-helped-create-thanos-avengers-infinity-war.jpg?itok=aBpL4XP-" alt="">
        <div class="header-component"><MarvelCardsHeader /></div>
    </div>
</template>

<script>
import MarvelCardsHeader from '@/components/MarvelCardsHeader.vue'

export default {
    name: 'marvelCardsMain',
    components: {
        MarvelCardsHeader
    }
}
</script>

<style lang="scss" scoped>
img {
    z-index: 0;
}

.header-component {
    z-index: 1;
}

div {
    width: 1300px;
    margin-left: auto;
    margin-right: auto;
}
</style>