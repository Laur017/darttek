<template>
    <div class="slider">
        <img src="../assets/web.png" alt="web">
        <p>Web Design</p>
        <img src="../assets/iphone.png" alt="iphone">
        <p>App Design</p>
        <img src="../assets/support.png" alt="support">
        <p>Support</p>
        <img src="../assets/ai.png" alt="ai">
        <p>Artificial Intelligence</p>
        <img src="../assets/git.png" alt="git">
        <p>Systems Integration</p>
        <img src="../assets/code.png" alt="code">
        <p>Software Development</p>
        <img src="../assets/cube.png" alt="cube">
        <p>Augmented & Virtual Reality Solutions</p>
        <img src="../assets/paint.png" alt="paint">
        <p>Branding</p>
        <img src="../assets/web.png" alt="web">
        <p>Web Design</p>
        <img src="../assets/iphone.png" alt="iphone">
        <p>App Design</p>
        <img src="../assets/support.png" alt="support">
        <p>Support</p>
        <img src="../assets/ai.png" alt="ai">
        <p>Artificial Intelligence</p>
        <img src="../assets/git.png" alt="git">
        <p>Systems Integration</p>
    </div>
</template>
<script></script>
<style>
.slider{
    width: calc(25rem * 26);
    background-color: var(--red);
    color: white;
    display: flex;
    align-items: center;
    overflow-y: hidden;
    font-size: 5rem;
    gap: 5rem;
    padding: 1rem 0;
    font-weight: 700;
    animation: slide 35s linear infinite;
    img{
        width: 5rem;
    }
    .star{
        padding-top: 1.5rem;
        font-size: 7rem;
    }
}


@keyframes slide {
    0% {
        transform: translateX(0)
    }

    100% {
        transform: translateX(calc(-25rem * 16.18))
    }
}
</style>