<template>
    <nav class="navigation">
        <div class="navigation-left">
            <img src="../assets/logo.png" alt="logo">
        </div>
        <div class="navigation-center">
            <a href="#">Services</a>
            <a href="#">Projects</a>
            <a href="#">Careers</a>
        </div>
        <div class="navigation-right">
            <button class="action-btn">Contact Us</button>
        </div>
    </nav>
</template>
<script></script>
<style>
.navigation{
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    padding: 3rem 10%;
}
.navigation-left{
    width: 33%;
    img{
        width: 75%;
        filter: drop-shadow(0 0 0.05rem var(--gray));
    }
}
.navigation-center{
    width: 33%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 3rem;

    a{
        all: unset;
        font-size: 2rem;
        letter-spacing: 1px;
        cursor: pointer;
        transition: all .3s ease;

        &:hover{
            color: var(--red);
        }
    }
}
.navigation-right{
    width: 33%;
    display: flex;
    align-items: center;
    justify-content: center;

}
</style>