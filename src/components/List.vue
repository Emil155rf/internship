<script>
export default {
    props: {
        title: String,
        description: String,
    }
}

</script>


<template>
    <div class="intern-list">
        <ul>
            <div class="list-1">
                <h1>{{ title }}</h1>
                <p>{{ description }}</p>
            </div>
        </ul>
    </div>



</template>



<style scoped>
.intern-list {
    display: flex;
    align-items: center;
    overflow: hidden;

}
ul {
    margin: 0; 
    padding: 0 0;
}
h1 {
    font-family: 'Mac';
    font-weight: 800;
    font-size: 25px;
}
p {
    font-size: 16px;

}
.list-1 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 20px 0;
    border-top: 2px solid hsla(0, 0%, 100%, .94);

}


</style>
