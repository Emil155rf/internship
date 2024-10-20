<script>
export default {
    props: {
        title: String,
    }

}


</script>


<template>

    <div class="selection-list">
        <ul>
            <div class="list-2">
                <h1>{{ title }}</h1>
            </div>
        </ul>
    </div>

</template>


<style scoped>
.selection-list {
    display: flex;
    align-items: center;
    overflow: hidden;
    color: hsla(0, 0%, 100%, .94);


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

.list-2 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 20px 0;
    border-top: 2px solid hsla(0, 0%, 100%, .94);

}
</style>