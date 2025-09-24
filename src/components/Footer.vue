<template>
    <div class="footer">
        <div class="footer-top">
            <div class="footer-top-left">
                <img src="../assets/logo.png" alt="logo">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ab natus ipsam corrupti sunt a velit</p>
                <div class="navigation-footer">
                    <a href="#">Services</a>
                    <a href="#">Projects</a>
                    <a href="#">Careers</a>
                </div>
            </div>
            <div class="footer-top-right">
                <h3>Contact</h3>
                <div>
                    <p><span><img src="../assets/phone.png" alt="phone"></span>+356 79901808</p>
                    <p><span><img src="../assets/email.png" alt="email"></span>info@darttek.com</p>
                    <p><span><img src="../assets/pin.png" alt="maps"></span>Suite 5, Level 3, Fafner House, Triq Nazzjonali, Hamrun HMR 9011, Malta</p>
                </div>
            </div>
        </div>
        <div class="footer-down">
            <div class="footer-down-left">
                <p>© 2025 Darttek. All rights reserved.</p>
            </div>
            <div class="footer-down-right">
                <div><img src="../assets/fb.png" alt="facebook"></div>
                <div><img src="../assets/linkedin.png" alt="linkedin"></div>
            </div>
        </div>
    </div>
</template>
<script></script>
<style>
.footer{
    background-color: var(--gray);
    color: white;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    padding: 1% 10%;
}

.footer-top{
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
}

.footer-top-left{
    display: flex;
    flex-direction: column;
    gap: 3rem;
    align-items: flex-start;
    img{
        width: 20%;
    }
    p{
        width: 50%;
        font-size: 2rem;
        color: rgba(255, 255, 255, 0.7);
    }
}
.navigation-footer{
    width: 33%;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 3rem;
    color: white;

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

.footer-top-right{
    display: flex;
    flex-direction: column;
    gap: 3rem;
    h3{
        font-size: 3rem;
    }
    div{
        display: flex;
        flex-direction: column;
        gap: 1rem;
        p{
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 2rem;
            width: 85%;
        }
        img{
            width: 3rem;
        }
    }
}

.footer-down{
    padding-top: 2%;
    border-top: 1px solid white;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .footer-down-left{
        p{
            font-size: 2rem;
            color: rgba(255, 255, 255, 0.75);
        }
    }

    .footer-down-right{
        display: flex;
        align-items: center;
        gap: 2rem;
        div{
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 1rem;
            border-radius: 50%;
            cursor: pointer;
            background-color: rgba(255, 255, 255, 0.75);
            transition: all .3s ease;

            &:hover{
                background-color: rgba(255, 255, 255, 1);
            }
            img{
                width: 2rem;
            }
        }
    }
}
</style>