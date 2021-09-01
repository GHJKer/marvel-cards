<template>
    <div class="header">
        <div class="header-img">
          <img src="https://images.vectorhq.com/images/previews/cd8/marvel-logo-psd-444569.png" alt="">  
        </div>
        <div class="btn-group">
            <button>MOVIES</button>
            <button>CHARACTERS</button>
            <button><a href="https://www.bbc.com/news">NEWS</a></button>
        </div>
        <div class="reg-group">
            <button>LOG IN</button>
            <button>SIGN UP</button>
        </div>
    </div>
</template>

<script>

export default {
    name: 'MarvelCardsHeader'
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300&display=swap');

.header {
    padding-top: 20px;
    display: flex;
    justify-content: space-between;
}

.btn-group {
    width: 350px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.reg-group {
    width: 200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

button {
    border: none;
    font-family: 'Noto Sans JP', sans-serif;
    font-weight: 700;
    color: white;
    background-color: transparent;
    cursor: pointer;
}

button:hover {
	background: rgba(0,0,0,0);
	color: #3a7999;
	box-shadow: inset 0 0 0 3px #3a7999;
    transition: all 0.5s ease;
}

a {
    text-decoration: none;
    color: white
}

img {
    height: 50px;
}

.bd {
    border: 1px solid red;
}
</style>