<script>
import Header from './components/Header.vue';
import Intern from './components/Intern.vue';
import List from './components/List.vue';
import DirectionTitle from './components/DirectionTitle.vue';
import Direction from './components/Direction.vue';
import Selection from './components/Selection.vue';
import SelectionList from './components/SelectionList.vue';
import Stage from './components/Stage.vue';
import StageList from './components/StageList.vue';

export default {
  components: {
    Header,
    Intern,
    List,
    DirectionTitle,
    Direction,
    Selection,
    SelectionList,
    Stage,
    StageList,


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
    <Direction />
  </div>
  <div class="selection-inner">
    <div class="container selection-container">
      <Selection />
      <SelectionList title="Хочешь создавать тренды и развивать банковскую индустрию" />
      <SelectionList title="Будешь стажироваться в Альфа‑Банке от 3 месяцев" />
      <SelectionList title="Можешь работать от 20 часов в неделю" />
      <Stage />
      <div class="stage-num">
        <StageList num="1" title="Отклик" description="Выбери направление и заполни заявку" />
        <StageList num="2" title="Тестирование" description="Выполни небольшое тестовое задание" />
        <StageList num="3" title="Собеседование" description="Пройди интервью с руководителем" />
        <StageList num="4" title="Оффер" description="Мы приглашаем тебя и ждём в команде!" />
      </div>
    </div>
  </div>









</template>

<style scoped>
.intern-container {
  background-color: red;
  color: hsla(0, 0%, 100%, .94);
  padding: 4em 0 4em 0;

}

.list-container {
  padding: 4em 0 5em 0;
  min-height: 40em;
}

.selection-inner {
  background-color: #FF34C6;
}

.selection-container {
  padding: 4em 0 4em 0;
}

.stage-num {
  display: flex;

}

@media screen and (max-width: 1200px) {
  .stage-num {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  
}

@media screen and (max-width: 850px) {
  .stage-num {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  
}


@media screen and (max-width: 550px) {
  .stage-num {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
  
}




</style>
