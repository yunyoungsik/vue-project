<script setup>
import { footerText } from "@/constants/index"
</script>

<template>
    <footer id="footer" role="contentinfo">
        <div class="footer__inner">
            <h2 class="footer__text">
                <div>yunyoungsik</div>
                <span>@0-SIK</span>
            </h2>
            <div class="footer__info">
                <div class="left">
                    <div class="title">
                        <a href="mailto:yunyoungsik@kakao.com">MAIL</a>
                    </div>
                    <p class="desc">누르시면 메일을 보내실 수 있습니다.</p>
                </div>
                <div class="right">
                    <h3>social</h3>
                    <ul>
                        <li v-for="(fot, key) in footerText" :key="key">
                            <a :href="fot.link">{{ fot.linkName }}</a>
                            <em>{{ fot.desc }}</em>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="footer__right">
                &copy; 2023 0-SIK<br />
                이 사이트는 비트를 이용하여 제작하였습니다.
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
#footer {
    width: 100%;
}

.footer__inner {
    padding: 1vw;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: var(--black);
    color: var(--black100);
    font-family: var(--mainKor-font);
    text-transform: uppercase;
}

.footer__text {
    width: 20%;
    text-align: center;
    font-size: 2rem;
    font-weight: 700;
}

.footer__text span {
    display: block;
    font-size: 1rem;
}

.footer__info {
    width: 80%;
    display: flex;
    justify-content: space-between;
    font-size: 1rem;
    padding: 0 1vw;
}

.footer__info .left {
    display: flex;
}

.footer__info .right h3 {
    font-weight: bold;
}

.footer__info li {
    margin-bottom: 0.5vw;
}

.footer__info a {
    background-color: var(--mainBg-color);
    color: var(--black);
    padding: 0.2vw 0.5vw;
    border-radius: 1vw;
    font-size: 0.8rem;
    margin-right: 0.3vw;
}

.footer__right {
    width: 20%;
    font-size: 0.8rem;
}
</style>