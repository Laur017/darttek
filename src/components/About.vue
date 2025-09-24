<template>
    <div class="about">
        <div class="about-left">
            <div class="about-left-up">
                <h3><span></span>Who we are</h3>
                <h1>We are <span>professionals</span></h1>
                <p>We share know-how, split risks and fully commit ourselves. We set goals and manage every aspect of every process to get there. We take pride in our skills and we specialize in a wide range of technologies.</p>
                <button>Learn More</button>
            </div>
            <div ref="aboutSection" class="about-left-down">
                <h3 v-if="visible">
                    10+
                <span>Years Of Experience</span>
                </h3>
                <h3 v-if="visible">
                    30+
                <span>Happy Clients</span>
                </h3>
                <h3 v-if="visible">
                    99%
                <span>Client Satisfaction</span>
            </h3>
            </div>
        </div>
        <div class="about-right">
            <div>
                <img src="../assets/we.avif" alt="we">
                <p>Our Projects</p>
            </div>
        </div>
    </div>
</template>

<script setup>
import NumberFlow from '@number-flow/vue'
import { ref, onMounted, onUnmounted } from 'vue'

const aboutSection = ref(null)
const visible = ref(false)

let observer

onMounted(() => {
  observer = new IntersectionObserver(
    (entries) => {
      if (entries[0].isIntersecting) {
        visible.value = true
        observer.unobserve(aboutSection.value)
      }
    },
    { threshold: 0.3 }
  )

  if (aboutSection.value) {
    observer.observe(aboutSection.value)
  }
})

onUnmounted(() => {
  if (observer && aboutSection.value) {
    observer.unobserve(aboutSection.value)
  }
})
</script>

<style>
.about{
    display: flex;
    align-items: center;
    padding: 5% 0;
    .about-left{
        width: 50%;
        display: flex;
        flex-direction: column;
        gap: 5rem;

        .about-left-up{
            align-self: center;
            width: 60%;
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

            p{
                font-size: 3rem;
            }

            button{
                margin-top: 3rem;
                padding: 1rem 3rem;
                font-family: inherit;
                font-size: 3rem;
                background-color: transparent;
                border: 2px solid var(--gray);
                color: var(--gray);
                cursor: pointer;
                transition: all .3s ease;

                &:hover{
                    background-color: var(--red);
                    color: white;
                    border: 2px solid var(--red);
                }
            }
        }

        .about-left-down{
            width: 70%;
            background-color: var(--red);
            display: flex;
            align-items: center;
            justify-content: flex-end;
            color: white;
            gap: 5rem;
            padding: 1rem 10% 1rem 0;
            h3{
                display: flex;
                flex-direction: column;
                align-items: center;
                font-size: 5rem;
                font-weight: 700;
            }
            span{
                font-size: 2rem;
                font-weight: 300;
            }
        }
    }
    .about-right{
        width: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        div{
            width: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 2rem;
            background-color: var(--red);
            padding: 2rem;

            p{
                font-size: 3rem;
                color: white;
                cursor: pointer;
            }
        }
        img{
            width: 100%;
            object-fit: cover;
        }
    }
}
</style>