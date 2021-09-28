<template>
    <div class="item-card">
        <div class="img-container">
            <img class="card-img"
            :src="imgUrl"
            >
        </div>
        <div class="character-info">
            <span>Имя: {{ name }}</span><br>
            <span>Прозвище: {{ nickName }}</span><br>
            <span>Раса: {{ race }}</span><br>
            <span>Способности: {{ power }} </span><br>
            <span>Пол: {{ gender }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MarvelCardsItem',
    props: ['imgUrl', 'name', 'nickName', 'race', 'power', 'gender'],

}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300&display=swap');

.item-card {
    width: 200px;
    border: 1px solid red;
    color: white;
}

.character-info {
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 700;
}

.img-container {
    width: 200px;
    height: 200px;
}

img {
    height: 100%;
    width: 100%;
    object-fit: cover;
}
</style>