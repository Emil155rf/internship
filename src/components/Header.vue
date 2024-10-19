<template>
    <div class="header-main">
        <div class="container">
            <div class="header">
                <div class="header-photo">
                    <img class="header-img" src="../assets/images/D_logo_white.svg" alt="">
                </div>
                <div class="header-row">
                    <ul class="sp">
                        <div class="dropdown">
                            <a class="dropBtn header__a" href="">Студенты</a>
                            <div class="dropdown-content">
                                <h1>Карьера</h1>
                                <a href="">Альфа Амбассадоры</a>
                                <a id="int" href="">Стажировки</a>
                                <a href="">Старт карьеры</a>

                                <div class="line"></div>

                                <h1>Образовательные проекты</h1>
                                <a href="">Магистратура МФТИ</a>
                                <a href="">Магистратура НИУ ВШЭ</a>
                                <a href="">Магистратура РУДН</a>
                                <a href="">Онлайн-курсы</a>

                                <div class="line"></div>

                                <h1>Мероприятия</h1>
                                <a href="">Альфа Движ</a>
                                <a href="">Альфа-Среда</a>
                            </div>
                        </div>
                        <div class="dropdown">
                            <a class="dropBtn header__a" href="">Преподаватели</a>
                            <div class="dropdown-content">
                                <h1>Образовательные проекты</h1>
                                <a href="">Искусственный интеллект Альфа‑Банк и ИТМО</a>
                                <a href="">Онлайн-курсы</a>
                                <a href="">Цифровая кафедра</a>
                                <a href="">Alfa Campus</a>

                            </div>
                        </div>
                        <div><a class="dropBtn header__a" href="">Партнёрство с вузами</a></div>
                    </ul>
                </div>
            </div>
            <div class="header-text">
                <div class="header-title"><img src="../assets/images/D_Title_560x252_160424.webp" alt=""></div>
                <p>Стажировка в Альфа-Банке для студентов со всей страны <br> Лучших возьмём на работу</p>
                <button id="lk-btn">Посмотреть стажировки</button>
            </div>
        </div>
    </div>







</template>

<script>
export default {
    data() {
        return {

        }
    },
    methods: {



    }


}


</script>


<style scoped>
.header-main {
    background-image: url(../assets/images/D_MainBan_1280x588_160424.webp);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-repeat: no-repeat;
    height: auto;

}

a {
    color: hsla(0, 0%, 100%, .94);

}

.header {
    top: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    width: 100%;
    padding-top: 44px;
    z-index: 10;

}

.header-row ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;

}



.header-text {
    display: flex;
    flex-direction: column;
    justify-content: left;
    align-items: flex-start;
    color: hsla(0, 0%, 100%, .94);
    margin: 10em 0 3em 0;

}


.header-title img {
    max-width: 560px;
    height: auto;
    width: 100%;
    vertical-align: middle;

}

.header-text p {
    font-size: 18px;
    line-height: 120%;
    margin-top: 1em;
}

.header-text button {
    margin-top: 1em;
    background-color: #ef3124;
    font-size: 16px;
    min-height: 48px;
    min-width: 224px;
    border-radius: 8px;
    border: none;
    color: hsla(0, 0%, 100%, .94);
    transition: .3s ease;

}

.header-text button:hover {
    background-color: #dc2e03;
}

.line {
    width: 90%;
    margin: 0 10px;
    height: .5px;
    background-color: #9999;
}

.dropdown {
    position: relative;
    display: inline-block;
    margin-right: 1.5em;
}

.dropbtn {
    background-color: #4CAF50;
    color: #fff;
    padding: 10px;
    font-size: 1rem;
    border: none;
    cursor: pointer;
    transition: .3s ease;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: hsla(0, 0%, 100%, .94);
    min-width: 250px;
    max-width: 300px;
    border-radius: 5px;
    font-size: 16px;
    box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
    z-index: 5;
}

.dropdown-content a {
    color: rgba(3, 3, 6, .88);
    padding: 12px 16px;
    text-decoration: none;
    display: block;
    border-radius: 10px;
}

#int {
    text-decoration: underline red 2px;
    text-underline-position: under;


}


.dropdown-content h1 {
    font-family: 'Styr';
    color: rgba(3, 3, 6, .88);
    padding: 22px 0 10px 16px;
    text-decoration: none;
    display: block;
    font-size: 18px;
    font-weight: 800;
    letter-spacing: -2px;
    border-radius: 10px;
}

.dropdown-content a:hover {
    color: #555555;
}

.dropdown:hover .dropdown-content {
    display: block;

}

.dropdown:hover .dropbtn {
    background-color: #3e8e41;
}


@media screen and (max-width: 500px) {
    
}
</style>
