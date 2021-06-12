<template>
    <footer class="bg-primary">
        <div class="footer-container">
            <div class="footer-nav d-flex justify-content-between">
                <div class="footer-nav__item d-flex flex-column">
                    <nuxt-link to="/employers"><b>Работодателям</b></nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                </div>
                <div class="footer-nav__item d-flex flex-column">
                    <nuxt-link to="/applicants"><b>Соискателям</b></nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                </div>
                <div class="footer-nav__item d-flex flex-column">
                    <nuxt-link to="/services"><b>Услуги</b></nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                    <nuxt-link to="#">test link</nuxt-link>
                </div>
            </div>
            <div class="social d-flex align-items-center justify-content-between">
                <a href="#"><img src="@/assets/img/vk.png" alt="vk"></a>
                <a href="#"><img src="@/assets/img/facebook.png" alt="facebook"></a>
                <a href="#"><img src="@/assets/img/telegram.png" alt="telegram"></a>
                <a href="#"><img src="@/assets/img/youtube.png" alt="youtube"></a>
            </div>
        </div>
        <div class="d-flex justify-content-center copyright"><span>2021 &#169; IT Manager</span></div>
    </footer>
</template>

<style scoped>
    .footer-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .copyright {
        color: #fff;
    }

    .social {
        width: 180px;
    }

    .social img {
        width: 40px;
    }

    footer {
        padding: 10px 20px;
    }

    .footer-nav {

        max-width: 400px;
    }

    .footer-nav__item {
        margin: 0 20px;
    }

    .footer-nav__item a {
        color: rgba(255,255,255,.55);
        text-decoration: none;
    }

    .footer-nav__item a:hover {
        color: #fff;
        transition: .4s;
    }

    @media screen and (max-width: 633px) {
        .footer-container {
            display: flex;
            justify-content: center;
            color: green;
        }
        .social {
            margin: 20px 0;
        }
    }

    @media screen and (max-width: 453px) {
        .footer-nav {
            flex-wrap: wrap;
        }
    }
</style>