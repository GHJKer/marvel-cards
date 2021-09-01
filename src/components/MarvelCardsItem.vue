<template>
    <div class="item-card">
        <img 
        :src="imgUrl"
        width="300px"
        >
        <div class="character-info">
            <span>Имя: {{ name }}</span>
            <span>Прозвище: {{ nickName }}</span>
            <span>Раса: {{ race }}</span>
            <span>Способности: {{ power }} </span>
            <span>Пол: {{ gender }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MarvelCardsItem',
    data() {
        return {
            name: 'Тони Старк',
            nickName: 'Железный человек',
            race: 'Человек',
            power: 'Деньги, костюм железного человека, интеллект',
            gender: 'Мужской'
        }
    }
}
</script>

<style lang="scss">

.item-card {
    width: 300px;
    min-height: 300px;
    border: 1px solid red;
    color: white;
}

</style>