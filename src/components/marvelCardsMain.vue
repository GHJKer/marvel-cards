<template>
    <div class="container-container">
        <div class="main-container">
            <MarvelCardsHeader />
        </div>
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
.main-container {
    width: 1300px;
    margin-left: auto;
    margin-right: auto;
    min-height: 500px;
}

.container-container {
    background: url(https://www.awn.com/sites/default/files/styles/original/public/image/featured/1046202-sympathy-devil-how-digital-domain-helped-create-thanos-avengers-infinity-war.jpg?itok=aBpL4XP-);
}
</style>