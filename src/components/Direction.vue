<template>
    <div>
        <div class="direction-div">
            <button class="direction-button" v-for="(direction, index) in directions" :key="index" @click="showInternships(index)"
                :class="{ active: selectedDirection === index }">
                {{ direction.name }}
            </button>
        </div>
        <div class="internship-list">
            <ul>
                <li class="intern-list" v-for="(internship, index) in internships[selectedDirection]" :key="index">
                    <div class="intern-name">{{ internship.name }}</div>
                    <div class="description">{{ internship.description }}</div>
                    <div class="intern-buttons">
                        <button class="watch-intern">Посмотреть стажировки <i class="bi bi-chevron-right"></i></button>
                        <button class="watch-intern-2"> <i class="bi bi-info-circle-fill"></i></button>
                    </div>
                </li>

            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            directions: [
                {
                    name: "Аналитика",
                },
                {
                    name: "Безопасность",
                },
                {
                    name: "Маркетинг",
                },
                {
                    name: "Продажи",
                },
                {
                    name: "Стратегия",
                },
                {
                    name: "Менеджмент",
                },
                {
                    name: "Финансы",
                },
                {
                    name: "IT и цифровой бизнес",
                },
                {
                    name: "Data Science",
                },
            ],
            internships: [
                [
                    { name: 'Аналитика бизнес-процессов', description: 'Изучать ключевые процессы банка и искать способы их оптимизации' },
                    { name: 'Аналитика данных', description: 'Моделировать бизнес‑кейсы, писать документацию и считать доход' },
                    { name: 'Продуктовая аналитика', description: 'Анализировать продуктовые метрики и строить по ним дашборды' },
                    { name: 'Финансовая аналитика', description: 'Собирать, анализировать и интерпретировать финансовые показатели' },
                ],
                [
                    { name: 'Кибербезопасность', description: 'Прогнозировать и предотвращать угрозы кибербезопасности' },
                    { name: 'Техническая безопасность', description: 'Искать и анализировать уязвимости информационных систем' },
                ],
                [
                    { name: 'Маркетинг', description: 'Проводить маркетинговые исследования и тестировать коммуникации' },
                    { name: 'UX-редактор', description: 'Создавать интерфейсы и оптимизировать пользовательский опыт' },
                ],
                [
                    { name: 'Корпоративные продажи', description: 'Искать новых клиентов и создавать коммерческие предложения' },
                ],
                [
                    { name: 'Стратегия', description: 'Анализировать обратную связь от клиентов и оптимизировать процессы' },
                ],
                [
                    {
                        name: "Проектный менеджмент",
                        description: "Генерировать идеи, следить за сроками и реализацией проектов."
                    },
                    {
                        name: "Продуктовый менеджмент",
                        description: "Оценивать успешность продукта и менять его под потребности рынка"
                    }
                ],
                [
                    {
                        name: "Финансы",
                        description: "Оценивать риски, вести бюджет, анализировать отчетность."
                    }
                ],
                [
                    { name: 'Тестирование', description: 'Проводить ручное тестирование и анализировать поведение системы' },
                    { name: 'Backend-разработка', description: 'Создавать веб‑приложения и интегрировать их с системами банка' },
                    { name: 'Администрирование баз данных', description: 'Настраивать, обновлять, бэкапить и оптимизировать работу СУБД' },
                    { name: 'Frontend-разработка', description: 'Создание интерфейсов и разработка функционала веб‑приложений' },
                    { name: 'DevOps', description: 'Автоматизировать процессы и обеспечивать работу ПО' },
                    { name: 'Fullstack-разработка', description: 'Разрабатывать серверную и клиентскую часть веб‑приложений' },
                ],
                [
                    { name: 'Data Engineering', description: 'Парсить, анализировать и систематизировать большие объёмы данных' },
                    { name: 'Data Science', description: 'Анализировать данные, делать прогнозы и визуализировать тренды' },
                ],
            ],
            selectedDirection: 0
        }
    },
    methods: {
        showInternships(index) {
            this.selectedDirection = index
        }
    },
    created() {
        this.selectedDirection = 0
    },
    watch: {
        selectedDirection(newDirectionIndex) {
            console.log("Selected Direction changed to:", newDirectionIndex)
        }
    }
}
</script>

<style scoped>
div {
    color: hsla(0, 0%, 100%, .94);
}

ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    padding: 0 0;
}

li {
    display: flex;
    flex-direction: column;
}

.description {
    padding: 10px 0;
    color: hsla(0, 0%, 100%, .85);
    font-size: 15px;
}

.internship-list {
    padding: 10px 0;
}

.direction-div {
    display: flex;
    flex-direction: row;
    padding-bottom: 1em;
}


.direction-div button {
    margin-right: 1em;
    min-height: 3em;
    border-radius: 25px;
    padding: 10px;

    background-color: rgba(255, 255, 255, 0.15);
    color: hsla(0, 0%, 100%, .94);
    border: 1px solid hsla(0, 0%, 100%, .94);
}

.direction-button:hover {
    background-color: rgba(255, 255, 255, 0.18);
}

.direction-button:focus {
    background-color: hsla(0, 0%, 100%, .94);
    color: #333;
    transition: .2s ease;
}

.intern-list {
    border: 1px solid hsla(0, 0%, 100%, .94);
    padding: 10px 20px;
    border-radius: 25px;
    margin: 1em 1em .3em 0;


}

.intern-name {
    padding: 5px 0;
}
.intern-buttons {
    display: flex;
    justify-content: space-between;
    align-items: center
}

.watch-intern {
    background-color: #ff34c6;
    color: hsla(0, 0%, 100%, .94);
    margin: 5px 0;
    text-align: left;
    font-size: 15px;
    border-radius: 15px;
    padding: 0 10px;
    min-height: 2em;
    width: 14em;
}

.bi-chevron-right {
    position: relative;
    top: 1px;
}


.bi-info-circle-fill {
    color: hsla(0, 0%, 100%, .94);
}
.watch-intern-2 {
    background-color: transparent;
    font-size: 22px;
    position: relative;
    top: 3px;
}

</style>