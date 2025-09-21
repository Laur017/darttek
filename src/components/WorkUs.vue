<template>
    <div class="work">
        <div class="work-up">
            <h3><span></span>Why choose us</h3>
            <h1>Why Trust Us For Your IT Needs?</h1>
        </div>
        <div class="work-down">
            <div class="work-down-left">
                <img src="../assets/we.jpg" alt="work with us">
            </div>
            <div class="work-down-right">
                <div>
                    <img src="../assets/star.png" alt="star">
                    <h2>Quality</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates voluptas maiores sapiente eligendi eaque sunt minus assumenda</p>
                </div>
                <div>
                    <img src="../assets/bubble.png" alt="bubble">
                    <h2>Communication</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates voluptas maiores sapiente eligendi eaque sunt minus assumenda</p>
                </div>
                <div>
                    <img src="../assets/lock.png" alt="lock">
                    <h2>Security</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates voluptas maiores sapiente eligendi eaque sunt minus assumenda</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script></script>
<style>
.work{
    background-color: var(--gray);
    color: white;
    padding: 5% 10%;
}

.work-up{
    h3{
        display: flex;
        align-items: center;
        gap: 1rem;
        font-size: 3rem;
        span{
            display: block;
            background-color: var(--red);
            width: 3rem;
            height: .5rem;
        }
        color: rgba(var(--gray), 0.5);
    }
    h1{
        font-size: 6rem;
        span{
            color: var(--red);
        }
    }
}

.work-down{
    display: flex;
    align-items: center;
    gap: 5rem;

    .work-down-left{
        width: 50%;

        img{
            width: 100%;
            object-fit: cover;
            border-radius: 5rem;
        }
    }

    .work-down-right{
        width: 50%;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 5rem;

        div{
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            gap: .5rem;
            cursor: default;
            img{
                width: 4rem;
            }

            h2{
                font-size: 4rem;
                transition: all .3s ease;
            }

            p{
                font-size: 2rem;
                color: rgba(255, 255, 255, 0.7);
            }
            &:hover{
                h2{
                    color: var(--red);
                }
            }
        }
    }

}
</style>