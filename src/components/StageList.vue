<script>
export default {
    props: {
        title: String,
        description: String,

    }

}

</script>


<template>

    <div class="stage-steps">
        <h1>1</h1>
        <div class="stage-text">
            <h2>{{ title }}</h2>
            <p>{{ description }}</p>
        </div>

    </div>
</template>


<style scoped>
h1 {
    font-weight: 800;
    margin-bottom: 1em;
    letter-spacing: 1px;
    color: hsla(0, 0%, 100%, .94);
    font-size: 45px;
    color: rgb(21, 240, 21);
}

.stage-steps {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #0E0E0E;
    border: none;
    width: 266.25px;


}
</style>