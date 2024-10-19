<script>
import Header from './components/Header.vue';
import Intern from './components/Intern.vue';
import List from './components/List.vue';
import DirectionTitle from './components/DirectionTitle.vue';
import Direction from './components/Direction.vue';

export default {
  components: {
    Header,
    Intern,
    List,
    DirectionTitle,
    Direction,


  }
}




</script>

<template>
  <Header />
  <div class="intern-container">
    <Intern />
    <div class="container">
      <List title="Реальные задачи" description="Поработаешь над актуальными продуктами банка" />
      <List title="Гибкий график"
        description="Можно совмещать с учёбой. А на некоторых стажировках — работать удалённо" />
      <List title="Современный офис"
        description="IT-хабы в Москве, Санкт-Петербурге, Екатеринбурге и сезонный коворкинг в Сочи" />
      <List title="Наставник"
        description="Всю стажировку с тобой будет опытный ментор, который всегда готов прийти на помощь" />
    </div>
  </div>
  <div class="container list-container">
    <DirectionTitle />
    <Direction/>
  </div>








</template>

<style scoped>
.intern-container {
  background-color: red;
  color: hsla(0, 0%, 100%, .94);
  padding: 4em 0 4em 0;

} 
.list-container {
  padding: 4em 0 0 0;
  height: 40em;
}
</style>
