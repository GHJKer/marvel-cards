<template>
    <div class="container-container">
        <div class="main-container">
            <MarvelCardsHeader />
        </div>
        <MarvelCardsItem />
    </div>
</template>

<script>
import MarvelCardsHeader from '@/components/MarvelCardsHeader.vue'
import MarvelCardsItem from '@/components/MarvelCardsItem.vue'

export default {
    name: 'marvelCardsMain',
    components: {
        MarvelCardsHeader, MarvelCardsItem
    },
    data() {
        return {
            characters: [
                {
                name: 'Тони Старк',
                nickName: 'Железный человек',
                race: 'Человек',
                power: 'Деньги, костюм железного человека, интеллект',
                gender: 'Мужской'
            },
            {
                name: 'Гамора',
                nickName: 'Гамора',
                race: 'Зен-Хобери',
                power: 'Улучшеная физическая сила, мастер боевых искусств, мастер вооружения',
                gender: 'Женский'
            },
            {
                name: 'Танос',
                nickName: "Безумный титан",
                race: 'Вечный',
                power: 'Сверинтеллект, сверхсила, неуязвимость',
                gender: 'Мужской'
            },
            ]
        }
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