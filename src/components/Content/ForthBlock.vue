<template>
    <div class="main">
        <the-card v-for="card in cards" :card="card" :key="card.id"/>
    </div>
</template>

<script>
import TheCard from "./TheCard.vue";

export default {
    components: { TheCard },
    data() { 
        return{
            cards: [
                {
                    id: 0,
                    icon: 'target',
                    title: 'Наше обучение построено очень лаконично и просто',
                    text: 'Все занятия короткие по продолжительности для легкого восприятия и понимания. Мы даем в уроках только конкретику, без лишней теории и “воды”.'
                },
                {
                    id: 1,
                    icon: 'site',
                    title: 'Ко всем урокам есть дополнительные материалы',
                    text: 'Презентации, краткие инструкции, чек-листы и памятки по работе с маркетплейсами.'
                },
                {
                    id: 2,
                    icon: 'friends',
                    title: 'Наше обучение — практико-ориентированное',
                    text: 'Поэтому после прохождения уроков ты будешь выполнять задания, которые помогут тебе закрепить полученные знания на практике.'
                },
                {
                    id: 3,
                    icon: 'icons',
                    title: 'Создатели нашей Академии',
                    text: 'Действующие селлеры с большим опытом в продажах на маркетплейсах, эксперты компании stat4market, а также профессиональные лекторы и методологи.'
                },
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
.main {
    padding: 85px 0;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-gap: 5%;
}

@media (max-width: 768px){
    .main {
        grid-template-columns: 1fr 1fr;
        grid-gap: 60px;
    }
}
@media (max-width: 360px){
    .main {
        grid-template-columns: 1fr;
        grid-gap: 40px;
    }
}
</style>