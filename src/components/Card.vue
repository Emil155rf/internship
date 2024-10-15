<script>

export default {
    props: {
        image: String,
        title: String,
        description: String,
        cls: String,
        sale: String
    }


}






</script>


<template>

    <!-- <div class="container"> -->
    <div class="card__inner">
        <div class="cards">
            <div class="card">
                <img :src="image" alt="Example Image">
                <div class="card-buttons">
                    <button style="margin-right: .5em;" class="card__btn">{{ cls }}</button>
                    <button style="margin-right: .5em;" class="card__btn-2">{{ sale }}</button>
                </div>
                <div class="card-text">{{ title }}</div>
                <div class="card-text-2">{{ description }}</div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.card__inner {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 1300px;
}


.card {
    position: relative;
    width: 400px;
    height: 55vh;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
    border: none;
}

.card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.8s ease;
}

.card:hover img {
    transform: scale(1.1);
}

.card-text {
    text-transform: uppercase;
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    padding-bottom: 50px;
    color: #fff;
    background: linear-gradient(to top, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0));
    text-align: center;
    font-size: 2rem;
}

.card-text-2 {
    text-transform: uppercase;
    position: absolute;
    top: 28em;
    left: 0;
    width: 100%;
    padding: 20px;
    color: #fff;
    text-align: center;
    font-size: 1rem;
    letter-spacing: 1px;
}

.card-buttons {
    position: absolute;
    top: 10px;
    right: 85px;
    display: flex;
    gap: 10px;
}

.card__btn {
    background-color: #e84e0e;
}

.card__btn-2 {
    background-color: #272727;
}

.card__btn-3 {
    width: 90px;
    height: 90px;
    border-radius: 45px;
    background: transparent;
    border: 1px solid #fff;
    color: #fff;
    margin-top: 2.5em;
}

.card-buttons button {
    padding: 5px 10px;
    color: #fff;
    border: none;

    border-radius: 15px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}
</style>