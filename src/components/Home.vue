<template>
    <div class="home">
        <h1>Perfection <br />Has No Limits!</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatem et mollitia non ducimus impedit magni obcaecati eos, saepe incidunt atque? Placeat a voluptatibus nobis exercitationem necessitatibus aliquam labore fugit laboriosam.</p>
        <div class="home-buttons">
            <button class="action-btn">Explore More ></button>
            <a href="#">View All Services</a>
        </div>
    </div>
</template>

<script>
</script>

<style>
.home{
    background-image: url(../assets/home.png);
    object-fit: cover;
    padding: 10% 10%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 2rem;

    h1{
        font-size: 7rem;
        color: white;
    }
    p{
        width: 50%;
        color: rgba(255, 255, 255, 0.7);
        font-size: 3rem;
    }
}

.home-buttons{
    margin-top: 3rem;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 2rem;

    a{
        all: unset;
        color: white;
        font-size: 2rem;
        border-bottom: 1px solid white;
        cursor: pointer;
        transition: all .3s ease;

        &:hover{
            border: none;
            color: var(--red);
        }
    }
}
</style>