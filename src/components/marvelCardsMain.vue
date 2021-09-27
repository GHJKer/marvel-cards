<template>
    <div class="container-container">
        <div 
        class="main-container">
            <MarvelCardsHeader />
        </div>
        <div class="cards-container bd">
            <div
            v-for="(character, index) in characters"
            :key="index"
            >
            <MarvelCardsItem 
                :imgUrl="character.imgUrl"
                :name="character.name"
                :nickName="character.nickName"
                :race="character.race"
                :power="character.power"
                :gender="character.gender"
            />
        </div>
        </div>
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
                imgUrl: 'https://www.buro247.ru/thumb/670x830_0/images/senina/avengers-infinity-war-iron-man.jpg',
                name: 'Тони Старк',
                nickName: 'Железный человек',
                race: 'Человек',
                power: 'Деньги, костюм железного человека, интеллект',
                gender: 'Мужской'
            },
            {
                imgUrl: 'https://cellularnews.com/wp-content/uploads/2020/06/87-avengers-infinity-war-character-poster-gamora-325x485.jpg',
                name: 'Гамора',
                nickName: 'Гамора',
                race: 'Зен-Хобери',
                power: 'Улучшеная физическая сила, мастер боевых искусств, мастер вооружения',
                gender: 'Женский'
            },
            {
                imgUrl: 'https://static.toiimg.com/photo/msid-75390440/75390440.jpg?344550',
                name: 'Танос',
                nickName: "Безумный титан",
                race: 'Вечный',
                power: 'Сверинтеллект, сверхсила, неуязвимость',
                gender: 'Мужской'
            },
            {
                imgUrl: 'https://www.buro247.ru/thumb/670x830_0/images/senina/avengers-infinity-war-iron-man.jpg',
                name: 'Тони Старк',
                nickName: 'Железный человек',
                race: 'Человек',
                power: 'Деньги, костюм железного человека, интеллект',
                gender: 'Мужской'
            },
            {
                imgUrl: 'https://cellularnews.com/wp-content/uploads/2020/06/87-avengers-infinity-war-character-poster-gamora-325x485.jpg',
                name: 'Гамора',
                nickName: 'Гамора',
                race: 'Зен-Хобери',
                power: 'Улучшеная физическая сила, мастер боевых искусств, мастер вооружения',
                gender: 'Женский'
            },
            {
                imgUrl: 'https://static.toiimg.com/photo/msid-75390440/75390440.jpg?344550',
                name: 'Танос',
                nickName: "Безумный титан",
                race: 'Вечный',
                power: 'Сверинтеллект, сверхсила, неуязвимость',
                gender: 'Мужской'
            },
            {
                imgUrl: 'https://www.buro247.ru/thumb/670x830_0/images/senina/avengers-infinity-war-iron-man.jpg',
                name: 'Тони Старк',
                nickName: 'Железный человек',
                race: 'Человек',
                power: 'Деньги, костюм железного человека, интеллект',
                gender: 'Мужской'
            },
            {
                imgUrl: 'https://cellularnews.com/wp-content/uploads/2020/06/87-avengers-infinity-war-character-poster-gamora-325x485.jpg',
                name: 'Гамора',
                nickName: 'Гамора',
                race: 'Зен-Хобери',
                power: 'Улучшеная физическая сила, мастер боевых искусств, мастер вооружения',
                gender: 'Женский'
            },
            {
                imgUrl: 'https://static.toiimg.com/photo/msid-75390440/75390440.jpg?344550',
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
    width: 90%;
    margin-left: auto;
    margin-right: auto;
}

.container-container {
    background: url(https://www.awn.com/sites/default/files/styles/original/public/image/featured/1046202-sympathy-devil-how-digital-domain-helped-create-thanos-avengers-infinity-war.jpg?itok=aBpL4XP-);
    background-size: cover;
}

.cards-container {
    padding-top: 20px;
    width: 90%;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.bd {
    border: 1px solid red;
}
</style>