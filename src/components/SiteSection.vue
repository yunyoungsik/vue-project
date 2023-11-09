<script setup>
import { siteText } from "@/constants/index"
</script>

<template>
    <section id="site">
        <div class="site__inner">
            <div class="site__title">
                site coding <em>작업물</em>
            </div>
            <div class="site__wrap">
                <div v-for="(site, key) in siteText" :key="key" :class="'siteitem s' + (key + 1)">
                    <span class="num">{{ key + 1 }}</span>
                    <div class="text">
                        <div>{{ site.text[0] }}</div>
                        <div>{{ site.text[1] }}</div>
                        <div>{{ site.text[2] }}</div>
                    </div>
                    <h3 class="title">
                        {{ site.title }}
                    </h3>
                    <div class="btn">
                        <a href="site.view">view</a>
                        <a href="site.code">code</a>
                    </div>
                    <div class="info">
                        <span>{{ site.info[0] }}</span>
                        <span>{{ site.info[1] }}</span>
                        <span>{{ site.info[2] }}</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.site__inner {
    padding: 1vw;
}

.site__title {
    position: sticky;
    top: 65px;
    left: 0;
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

.site__title em {
    font-family: var(--mainKor-font);
    font-size: 1rem;
    color: var(--mainBg-color);
    font-weight: 400;
}

.siteitem {
    width: 100%;
    padding: 2vw;
    background-color: var(--black);
    color: var(--white);
    position: sticky;
    left: 0;
}

.siteitem.s1 {
    top: 180px;
}

.siteitem.s2 {
    background-color: var(--subBg100);
    top: 200px;
}

.siteitem.s3 {
    background-color: var(--black);
    top: 220px;
}

.siteitem.s4 {
    background-color: var(--subBg100);
    top: 240px;
}

.siteitem .num {
    display: inline-block;
    font-family: var(--mainNum-font);
    font-size: 5rem;
    margin-bottom: 1vw;
}

.siteitem .text {
    font-family: var(--mainEng-font);
    font-size: 3rem;
    font-weight: 700;
    padding: 3vw 0;
    text-transform: uppercase;
    text-align: center;
    box-sizing: border-box;
}

.siteitem .text div:nth-child(2) {
    color: var(--mainBg-color);
}

.siteitem .title {
    color: var(--mainBg-color);
    font-weight: 700;
    margin-bottom: 0.5vw;
    position: relative;
    margin-left: 1vw;
}

.siteitem .title::before {
    position: absolute;
    content: '';
    width: 5px;
    height: 5px;
    top: 50%;
    left: -1vw;
    transform: translateY(-50%);
    background-color: var(--mainBg-color);
}

.siteitem .btn a {
    display: inline-block;
    width: 7vw;
    font-size: 0.8rem;
    font-weight: 700;
    text-align: center;
    padding: 0.3vw 1vw;
    border-radius: 5vw;
    margin-bottom: 1vw;
    box-sizing: border-box;
}

.siteitem .btn a:nth-child(1) {
    color: var(--black500);
    background-color: var(--mainBg-color);
    margin-right: 1vw;
}

.siteitem .btn a:nth-child(1):hover {
    background-color: var(--mainBg-hover);
}

.siteitem .btn a:nth-child(2) {
    color: var(--black500);
    background-color: var(--white);
}

.siteitem .btn a:nth-child(2):hover {
    background-color: var(--white100);
}

.siteitem .info span {
    display: block;
    text-transform: uppercase;
    font-family: var(--mainNum-font);
    font-weight: 700;
}
</style>