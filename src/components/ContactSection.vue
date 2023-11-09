<template>
    <section id="contact">
        <div class="contact__inner">
            <div class="contact__line" aria-hidden="true">
                <span>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                </span>
            </div>
            <div class="contact__title">
                <div class="contact__text">
                    <div class="good">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0.5 0.5 16 16"
                            class="Appreciations-icon-Z4i Project-icon-qll" aria-hidden="true">
                            <path fill="none" d="M.5.5h16v16H.5z"></path>
                            <path
                                d="M.5 7.5h3v8h-3zM7.207 15.207c.193.19.425.29.677.293H12c.256 0 .512-.098.707-.293l2.5-2.5c.19-.19.288-.457.293-.707V8.5c0-.553-.445-1-1-1h-5L11 5s.5-.792.5-1.5v-1c0-.553-.447-1-1-1l-1 2-4 4v6l1.707 1.707z">
                            </path>
                        </svg>
                    </div>
                    <div class="contact__info">
                        <a href="#">MAIL : yunyoungsik@kakao.com</a>
                    </div>
                    <div class="contact__info__bottom">
                        <div class="icon">
                            <div class="good2">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0.5 0.5 16 16"
                                    class="Appreciations-icon-Z4i Project-icon-qll" aria-hidden="true">
                                    <path fill="none" d="M.5.5h16v16H.5z"></path>
                                    <path
                                        d="M.5 7.5h3v8h-3zM7.207 15.207c.193.19.425.29.677.293H12c.256 0 .512-.098.707-.293l2.5-2.5c.19-.19.288-.457.293-.707V8.5c0-.553-.445-1-1-1h-5L11 5s.5-.792.5-1.5v-1c0-.553-.447-1-1-1l-1 2-4 4v6l1.707 1.707z">
                                    </path>
                                </svg>
                                <span>777</span>
                            </div>
                            <div class="view">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" class="Project-icon-qll"
                                    aria-hidden="true">
                                    <path
                                        d="M8.5 3.5c-5 0-8 5-8 5s3 5 8 5 8-5 8-5-3-5-8-5zm0 7c-1.105 0-2-.896-2-2 0-1.106.895-2 2-2 1.104 0 2 .894 2 2 0 1.104-.896 2-2 2z">
                                    </path>
                                </svg>
                                <span>1.8k</span>
                            </div>
                            <div class="talk">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" class="Project-icon-qll"
                                    aria-hidden="true">
                                    <rect width="16" height="16" fill="none"></rect>
                                    <path
                                        d="M13 3H2C1.4 3 1 3.4 1 4v6l0 0c0 0.6 0.5 1 1 1h3v4h1l4-4h3c0.6 0 1-0.4 1-1l0 0V4C14 3.4 13.6 3 13 3z">
                                    </path>
                                </svg>
                                <span>777</span>
                            </div>
                        </div>
                        <p>게시 : 2023년11월06일</p>
                    </div>
                </div>
            </div>
            <div class="contact__line bottom" aria-hidden="true">
                <span>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                </span>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
#contact {
    width: 100%;
    height: 100vh;
}

.contact__inner {
    padding: 1vw;
}

.contact__line .line {
    display: block;
    width: 100%;
    height: 1px;
    background-color: var(--black);
    margin: 0.5vw 0;
}

.contact__line .line:nth-child(1) {
    height: 1px;
    margin: 0.1vw 0 0;
}

.contact__line .line:nth-child(2) {
    height: 2px;
    margin: 0.2vw 0 0;
}

.contact__line .line:nth-child(3) {
    height: 3px;
    margin: 0.3vw 0 0;
}

.contact__line .line:nth-child(4) {
    height: 4px;
    margin: 0.4vw 0 0;
}

.contact__line .line:nth-child(5) {
    height: 5px;
    margin: 0.5vw 0 0;
}

.contact__line .line:nth-child(6) {
    height: 6px;
    margin: 0.6vw 0 0;
}

.contact__line .line:nth-child(7) {
    height: 7px;
    margin: 0.7vw 0 0;
}

.contact__line.bottom .line:nth-child(1) {
    height: 7px;
    margin: 0.7vw 0 0;
}

.contact__line.bottom .line:nth-child(2) {
    height: 6px;
    margin: 0.6vw 0 0;
}

.contact__line.bottom .line:nth-child(3) {
    height: 5px;
    margin: 0.5vw 0 0;
}

.contact__line.bottom .line:nth-child(4) {
    height: 4px;
    margin: 0.4vw 0 0;
}

.contact__line.bottom .line:nth-child(5) {
    height: 3px;
    margin: 0.3vw 0 0;
}

.contact__line.bottom .line:nth-child(6) {
    height: 2px;
    margin: 0.2vw 0 0;
}

.contact__line.bottom .line:nth-child(7) {
    height: 1px;
    margin: 0.1vw 0 0;
}

.contact__text {
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

.contact__text .good {
    width: 6vw;
    height: 6vw;
    border-radius: 4vw;
    background-color: #0057ff;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 1vw;
}

.contact__text .good:hover {
    background-color: #014de6;
}

.contact__text .good svg {
    width: 3vw;
    fill: var(--white);
}

.contact__text .contact__info {
    margin-bottom: 2vw;
}

.contact__text .contact__info a {
    font-family: var(--mainKor-font);
    color: var(--white);
    display: block;
    font-size: 2rem;
}

.contact__info__bottom {
    color: var(--black100);
    font-family: var(--mainKor-font);
    font-size: 1rem;
}

.contact__info__bottom .icon {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 1vw;
}

.contact__info__bottom .good2,
.contact__info__bottom .view {
    margin-right: 1vw;
}

.contact__info__bottom svg {
    width: 1vw;
    fill: var(--black100);
}

.contact__info__bottom p {
    display: block;
    font-size: 1rem;
    color: var(--black100);
}
</style>