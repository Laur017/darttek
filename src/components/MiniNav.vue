<template>
    <nav class="mini-nav">
        <div class="mini-nav_left">
            <p><span><img src="../assets/phone.png" alt="phone"></span>+356 79901808</p>
            <p><span><img src="../assets/email.png" alt="mail"></span>info@darttek.com</p>
        </div>
        <div class="mini-nav_right">
            <div><img src="../assets/fb.png" alt="facebook"></div>
            <div><img src="../assets/linkedin.png" alt="linkedin"></div>
        </div>
    </nav>
</template>
<script></script>
<style>
.mini-nav{
    background-color: var(--gray);
    color: var(--background-color);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem 10%;
}

.mini-nav_left{
    display: flex;
    align-items: center;
    gap: 5rem;

    p{
        display: flex;
        align-items: center;
        font-size: 2rem;
        gap: 1rem;
    }
    span{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    img{
        width: 2rem;
    }
}
.mini-nav_right{
    display: flex;
    align-items: center;
    gap: 2rem;
    div{
        padding: 1rem;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
        background-color: rgba(255, 255, 255, 0.75);
            transition: all .3s ease;

            &:hover{
                background-color: rgba(255, 255, 255, 1);
            }
    }
    img{
        width: 2rem;
    }
}
</style>