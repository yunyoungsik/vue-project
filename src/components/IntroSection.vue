<template>
    <section id="intro">
        <div class="intro__inner">
            <h1 class="intro__title">
                frontend developer
            </h1>
            <div class="intro__lines" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>

            <div class="intro__text">
                <div class="text">
                    <div>talent is</div>
                    <div>found at the end of the</div>
                    <div>effort</div>
                </div>
                <div class="img">
                    <img src="../assets/img/img00.jpg" alt="프로필 이미지">
                </div>
            </div>

            <div class="intro__lines bottom" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Shrikhand&display=swap');

#intro {
    height: 100vh;
}

.intro__inner {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
    flex-direction: column;
    background-color: var(--mainBg-color);
    padding: 1vw;
}

.intro__title {
    font-size: 8.2vw;
    text-transform: uppercase;
    font-family: var(--mainPoint-font);
    color: var(--black);
    line-height: 0.6;
    letter-spacing: -0.2vw;
}

.intro__lines {
    display: block;
    width: 100%;
}

.intro__lines .line {
    display: block;
    width: 100%;
    height: 1px;
    background-color: var(--black);
    margin: 0.5vw 0;
}

.intro__lines .line:nth-child(1) {
    height: 1px;
    margin: 0.1vw 0 0;
}

.intro__lines .line:nth-child(2) {
    height: 2px;
    margin: 0.2vw 0 0;
}

.intro__lines .line:nth-child(3) {
    height: 3px;
    margin: 0.3vw 0 0;
}

.intro__lines .line:nth-child(4) {
    height: 4px;
    margin: 0.4vw 0 0;
}

.intro__lines .line:nth-child(5) {
    height: 5px;
    margin: 0.5vw 0 0;
}

.intro__lines .line:nth-child(6) {
    height: 6px;
    margin: 0.6vw 0 0;
}

.intro__lines .line:nth-child(7) {
    height: 7px;
    margin: 0.7vw 0 0;
}

.intro__lines.bottom {
    display: none;
}

.intro__lines.bottom .line:nth-child(1) {
    height: 7px;
    margin: 0.7vw 0 0;
}

.intro__lines.bottom .line:nth-child(2) {
    height: 6px;
    margin: 0.6vw 0 0;
}

.intro__lines.bottom .line:nth-child(3) {
    height: 5px;
    margin: 0.5vw 0 0;
}

.intro__lines.bottom .line:nth-child(4) {
    height: 4px;
    margin: 0.4vw 0 0;
}

.intro__lines.bottom .line:nth-child(5) {
    height: 3px;
    margin: 0.3vw 0 0;
}

.intro__lines.bottom .line:nth-child(6) {
    height: 2px;
    margin: 0.2vw 0 0;
}

.intro__lines.bottom .line:nth-child(7) {
    height: 1px;
    margin: 0.1vw 0 0;
}

.intro__text {
    background-color: var(--black);
    padding: 10vw 0;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    text-align: center;
    text-transform: uppercase;
    font-weight: 700;
    font-size: 3rem;
    line-height: 1.2;
    position: relative;
}

.intro__text .text {
    z-index: 1;
    padding: 0.5rem 4rem;
    color: var(--white);
    font-size: 3rem;
    text-decoration: underline;
    text-underline-position: under;
    background-color: rgba(0, 0, 0, .15);
    transition: opacity 0.3s;
}

.intro__text:hover .text {
    opacity: 0;
}

.intro__text .text div:nth-child(2) {
    color: var(--mainBg-color);
}

.intro__text .img {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    width: 17vw;
    height: 17vw;
    border-radius: 50%;
}

.intro__text .img img {
    width: 100%;
    vertical-align: top;
    filter: saturate(0);
    border-radius: 50%;
    transition: filter, transform 0.3s;
}

.intro__text:hover .img img {
    filter: saturate(1);
    transform: scale(130%);
}

@media(max-width: 1050px) {
    .intro__title {
        text-align: center;
        line-height: 0.7;
    }

}

@media(max-width: 800px) {
    .intro__inner {
        justify-content: center;
    }

    .intro__lines.bottom {
        display: block;
    }

    .intro__text .text {
        font-size: 1.5rem;
    }

    .intro__text .img {
        width: 20vw;
        height: 20vw;
    }

}
</style>