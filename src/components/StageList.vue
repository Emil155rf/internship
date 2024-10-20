<script>
export default {
    props: {
        num: String,
        title: String,
        description: String,

    }

}

</script>


<template>

    <div class="stage-steps">
        <h1>{{ num }}</h1>
        <div class="stage-text">
            <h2>{{ title }}</h2>
            <p>{{ description }}</p>
        </div>

    </div>
</template>


<style scoped>
h1 {
    font-weight: 800;
    margin: .1em .5em 1em .5em;
    color: hsla(0, 0%, 100%, .94);
    font-size: 55px;
    color: rgb(149, 240, 21);

}

.stage-steps {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #0E0E0E;
    border: none;
    width: 266.25px;
    border-radius: 25px;
    margin-right: 1em;



}

h2 {
    color: hsla(0, 0%, 100%, .94);
    margin: 1.5em 0 .2em 0;
    font-size: 22px;
    font-weight: 800;
}

p {
    font-size: 14px;
    color: hsla(0, 0%, 100%, .84);
    margin-bottom: 0.5em;




}
</style>