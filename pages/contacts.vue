<template>
    <section id="contacts" class="container contacts__section">
        <div class="contacts__title">
            <div class="contacts__title-text">Наши контакты</div>
        </div>

        <div class="contacts__info-block">
            <div class="contacts__info">
                <div class="address">
                    <address>
                        Астана, ул. Д. Кунаева 10. офис 2819. Бизнес центр Emerald Tower
                    </address>
                </div>
                <div class="phone">
                    <img src="/img/phone_black.svg" alt="" />
                    <a href="tel:+77770249314">+7 (777)-024-93-14</a>
                </div>
                <div class="email">
                    <img src="/img/email_black.svg" alt="" />
                    <a href="mailto:info@lorem ipsum">info@auratech.kz</a>
                </div>
                <div class="back_call">
                    <NuxtLink to="/application">
                        <button class="btn qq-button">Оставить заявку</button>
                    </NuxtLink>
                </div>
            </div>
            <div class="contacts__map">
                <img class="map-image" src="/img/map.jpeg" alt="img/" />
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.contacts__section {
    position: relative;
}

.contacts__info-block {
    display: flex;
}

.contacts__title-text {
    font-style: normal;
    font-weight: 500;
    font-size: 3.75em;
    line-height: 4em;
    text-transform: uppercase;
    color: #000000;
}

.contacts__info {
    width: 40%;
    padding: 5em 8em 5em 0;
}

.contacts__map {
    width: 829px;
    height: 631px;

    img {
        width: 100%;
        height: 100%;
    }

    ;
}

.contacts__info {
    .address {
        font-size: 1.5em;
        line-height: 1.5em;
        color: #000000;
    }

    .phone {
        margin-top: 1.3em;

        a {
            font-weight: 500;
            font-size: 20px;
            line-height: 32px;
            color: #000000;
        }
    }

    .email {
        margin-top: 2em;

        a {
            font-weight: 500;
            font-size: 20px;
            line-height: 32px;
            color: #000000;
        }
    }

    .back_call {
        margin-top: 2em;

    }

}

@media screen and (orientation: portrait) and (max-width: 880px) {
    .contacts__title-text {
        font-size: 2.2em;
        line-height: 2.2em;
    }

    .contacts__info-block {
        display: flex;
        flex-direction: column-reverse;
    }

    .contacts__map {
        width: 100%;
        height: auto;
    }

    .contacts__info {
        width: 100%;
        padding: 2em 0;
    }
}
</style>