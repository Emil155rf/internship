<script>
import Header from './components/Header.vue';
import Intern from './components/Intern.vue';
import List from './components/List.vue';
// import City from './components/City.vue';
// import Card from './components/Card.vue';

export default {
  components: {
    Header,
    Intern,
    List,

  }
}




</script>

<template>
  <Header />
  <div class="intern-container">
    <Intern />
    <div class="container">
      <List title="Реальные задачи" description="Поработаешь над актуальными продуктами банка" />
      <List title="Гибкий график" description="Можно совмещать с учёбой. А на некоторых стажировках — работать удалённо" />
      <List title="Современный офис" description="IT-хабы в Москве, Санкт-Петербурге, Екатеринбурге и сезонный коворкинг в Сочи" />
      <List title="Наставник" description="Всю стажировку с тобой будет опытный ментор, который всегда готов прийти на помощь" />
    </div>
  </div>
  <!-- <div class="container">
    <div class="crd">
      <Card image="/images/1721380564077-ee4e182dfd19649eff085ffe32702449.avif" title="СИМОНОВСКИЙ ВАЛ"
        description="дубровка" cls="Скоро старт продаж" sale="Бизнес-класс" />
      <Card image="/images/1726146895853-feee9edc8af1a8b31733998597fd189b.avif" title="amber city" description="беговая"
        cls="Старт продаж" sale="Премиум-класс" />
      <Card image="/images/1707758530724-164d1854af6e285fc6899b64ef59e7c2.avif" title="sky garden"
        description="тушинская" cls="Ипотека 5%" sale="Скидки до 15%" />
      <Card image="/images/616993a36814c_a0d4bf87c096de61370ca273ede526cd.avif" title="sydney city"
        description="звенигородская(2025)" cls="Скидки до 30%" sale="Рассрочка 0%" />
      <Card image="/images/62b5b50844792_c702c0d82fae4bfec6e89da9cbe30b44.avif" title="rotterdam"
        description="нагатинская" cls="Скидки до 25%" sale="Бизнес-класс" />
      <Card image="/images/1716280586030-99835b258d4a937807dad2babbe4083a.avif" title="the lake"
        description="ботанический сад" cls="Скидки до 30%" sale="Премиум-класс" />
      <Card image="/images/6169920bab15b_0f442c2587aba09d0d2c07b33d81eb74.avif" title="СИМОНОВСКИЙ ВАЛ"
        description="дубровка" cls="Скидки до 20%" sale="Премиум-класс" />
      <Card image="/images/5f7dd473d2d9e_6b1372d689c7d138d2f4ac3121909de9.avif" title="СИМОНОВСКИЙ ВАЛ"
        description="дубровка" cls="Скидки до 15%" sale="От 17600 р/месяц" />
      <Card image="/images/62f4e9b2dbeb7_7d8f1de45b261a6b6fca44754c1dc6cc.avif" title="СИМОНОВСКИЙ ВАЛ"
        description="дубровка" cls="Рассрочка 0%" sale="Юго-запад Москвы" />
    </div>
  </div>  -->







</template>

<style scoped>
.intern-container {
  background-color: red;
  color: hsla(0, 0%, 100%, .94);
  padding-top: 4em;
  min-width: 600px;
  width: 100%;
  /* height: auto; */

}


</style>
