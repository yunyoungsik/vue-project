<script setup>
import { skillText } from "@/constants/index"
</script>

<template>
    <section id="skill">
        <div class="skill__inner">
            <h2 class="skill__title">
                challenge <em>도전</em>
            </h2>
            <div class="skill__desc">
                <div v-for="(skill, key) in skillText" :key="key">
                    <span>{{ key + 1 }}</span>
                    <h3>{{ skill.title }}</h3>
                    <p>
                        {{ skill.desc }}
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.skill__inner {
    padding: 1vw;
    display: flex;
    justify-content: space-between;
}

.skill__title {
    position: sticky;
    top: 65px;
    left: 0;
    width: 48%;
    height: 12vw;
    padding: 2vw;
    background-color: var(--black);
    font-size: 5vw;
    color: var(--white);
    font-weight: 900;
    line-height: 1.6;
    text-transform: uppercase;
    font-family: var(--mainPoint-font);
}

.skill__title em {
    font-family: var(--mainKor-font);
    font-size: 1rem;
    color: var(--mainBg-color);
    font-weight: 400;
}

.skill__desc {
    width: 50%;
    padding: 2vw;
    background-color: var(--black);
    color: var(--white);
}

.skill__desc span {
    display: inline-block;
    font-family: var(--mainNum-font);
    font-size: 5rem;
    margin-bottom: 1vw;
}

.skill__desc h3 {
    font-size: 2rem;
    font-family: var(--mainKor-font);
    color: var(--mainBg-color);
    margin-bottom: 3vw;
}

.skill__desc p {
    font-size: 1rem;
    font-family: var(--mainKor-font);
    margin-bottom: 35vw;
}

@media(max-width: 800px) {
    .skill__inner {
        flex-direction: column;
    }

    .skill__title {
        width: 100%;
        margin-bottom: 10vw;
        height: auto;
        background: var(--black);
    }

    .skill__desc {
        width: 100%;
    }

    .skill__desc span {
        font-size: 8rem;
    }

    .skill__desc p {
        font-size: 1.2rem;
        margin-bottom: 55vw;
    }
}
</style>