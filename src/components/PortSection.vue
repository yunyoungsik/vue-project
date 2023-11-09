<script setup>
import { portText } from "@/constants/index"
</script>

<template>
    <section id="port">
        <div class="port__inner">
            <div class="port__title">
                portfolio <em>포트폴리오</em>
            </div>
            <div class="port__wrap">
                <div v-for="(port, key) in portText" :key="key" :class="'port__item p' + (key + 1)">
                    <span class="num">{{ key + 1 }}</span>
                    <a :href="port.view">
                        <svg xmlns="http://www.w3.org/2000/svg" width="32px" height="32px" viewBox="0 0 24 24">
                            <g>
                                <path
                                    d="M13.85,11.65c0.2,0.18,0.19,0.52,0,0.7l-3,3c-0.19,0.2-0.5,0.19-0.7,0c-0.2-0.18-0.19-0.52,0-0.7
                                                                                                                            L12.79,12l-2.64-2.65c-0.2-0.19-0.19-0.5,0-0.7c0.18-0.2,0.52-0.19,0.7,0L13.85,11.65z" />
                                <path
                                    d="M12,2.067c5.477,0,9.933,4.456,9.933,9.933S17.477,21.933,12,21.933S2.067,17.477,2.067,12
                                                                                                                            S6.523,2.067,12,2.067z M12,20.933c4.926,0,8.933-4.007,8.933-8.933S16.926,3.067,12,3.067S3.067,7.074,3.067,12
                                                                                                                            S7.074,20.933,12,20.933z" />
                            </g>
                        </svg>
                        <img :src="port.img" :alt="port.name">
                    </a>
                    <h3 class="title">{{ port.title }}</h3>
                    <p class="desc">
                        {{ port.desc }}
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import gsap from "gsap";
import scrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(scrollTrigger);

export default {
    mounted: function () {
        this.scrollAnimation();
    },
    methods: {
        scrollAnimation() {
            const horSection = gsap.utils.toArray(".port__item");

            gsap.to(horSection, {
                xPercent: -120 * (horSection.length - 1),
                ease: "none",
                scrollTrigger: {
                    trigger: "#port",
                    start: "top 65",
                    end: "+=3000",
                    pin: true,
                    scrub: 1,
                    markers: true,
                    invalidateOnRefresh: true,
                    anticipatePin: 1,
                }
            });
        }
    }
}
</script>

<style lang="scss">
#port {
    width: 100%;
    overflow: hidden;
}

.port__inner {
    padding: 1vw;
}

.port__wrap {

    display: flex;
    flex-wrap: wrap;
    width: 7000px;
}

.port__title {
    /* position: sticky;
    top: 65px;
    left: 0; */
    width: 100%;
    height: auto;
    padding: 2vw;
    background-color: var(--black);
    font-size: 2rem;
    color: var(--white);
    font-weight: 900;
    line-height: 1.6;
    text-transform: uppercase;
    font-family: var(--mainPoint-font);
    box-sizing: border-box;
}

.port__title em {
    font-family: var(--mainKor-font);
    font-size: 1rem;
    color: var(--mainBg-color);
    font-weight: 400;
}

.port__item {
    width: 500px;
    height: 70vh;
    padding: 1vw;
    margin-right: 20px;
    background-color: var(--black);
    position: relative;
    border-top: 1px solid rgba(255, 255, 255, 0.15);
    box-sizing: border-box;
}

.port__item .num {
    position: absolute;
    left: 1.5vw;
    top: 1.5vw;
    color: var(--white);
    background-color: rgba(0, 0, 0, 0.5);
    border-radius: 50%;
    width: 2rem;
    height: 2rem;
    font-size: 1rem;
    text-align: center;
    line-height: 2rem;
    z-index: 1;
}

.port__item a {
    filter: saturate(1);
    filter: saturate(0);
    transition: all 0.5s;
    opacity: 50%;
    position: relative;
    overflow: hidden;
    display: block;
}

.port__item a:hover {
    filter: saturate(1);
    opacity: 100%;
}

.port__item a svg {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    fill: var(--white);
    transition: all 0.3;
}

.port__item a:hover svg {
    opacity: 0;
}

.port__item a img {
    width: 100%;
    aspect-ratio: 16/9;
    object-fit: cover;
    object-position: center;
    /* default: center */
}

.port__item .title {
    margin-top: 1vw;
    font-size: 1rem;
    font-weight: 700;
    color: var(--mainBg-color);
    position: relative;
    margin-left: 1vw;
}

.port__item .title::before {
    position: absolute;
    content: '';
    width: 5px;
    height: 5px;
    top: 50%;
    left: -1vw;
    transform: translateY(-50%);
    background-color: var(--mainBg-color);
}

.port__item .desc {
    font-size: 1rem;
    margin-top: 0.5vw;
    color: var(--white);
}
</style>