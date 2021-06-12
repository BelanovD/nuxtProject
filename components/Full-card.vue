<template>
    <div>
        <h1>Анкета</h1>
        <nuxt-link to="/employers" class="back-link">Назад</nuxt-link>
        <div class="d-flex questionnaire">
            <div class="flex-left">
                <div class="applicant-photo">
                    <img src="@/assets/img/belanov.jpg" alt="{}">
                </div>
                <p class="value-know"><b>Ценность по знаниям:</b></p>
                <p class="value-know"><b>Ценность по ЗП:</b></p>
            </div>
            <div class="flex-right d-flex flex-column justify-content-between">
                <div class="d-flex flex-right__item">
                    <p class="title"><b>Имя:</b></p>
                    <p class="right">Lorem, ipsum.</p><br>
                </div>
                <div class="d-flex flex-right__item">
                    <p class="title"><b>Стэк:</b></p>
                    <p class="right">About me: Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci sunt quia iure quibusdam enim saepe. Distinctio itaque quibusdam iusto sapiente!</p>
                </div>
                <div class="d-flex flex-right__item">
                    <p class="title"><b>Hard skills:</b></p>
                    <p class="right">Lorem, ipsum.</p><br>
                </div>
                <div class="d-flex flex-right__item">
                    <p class="title"><b>Soft skills:</b></p>
                    <p class="right">Lorem, ipsum.</p><br>
                </div>
                <div class="d-flex flex-right__item">
                    <p class="title"><b>О себе:</b></p>
                    <p class="right">About me: Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci sunt quia iure quibusdam enim saepe. Distinctio itaque quibusdam iusto sapiente!</p>
                </div>
                <div class="d-flex flex-right__item">
                    <p class="title"><b>Способ связи:</b></p>
                    <p class="right">test@gmail.com</p><br>
                </div>
            </div>
        </div>
        <div class="d-flex justify-content-center">
                    <div class="d-flex justify-content-between tehnology">
                        <p>HTML</p>
                        <p>CSS</p>
                        <p>JS</p>
                    </div>
                </div>
            <div class="d-flex flex-column align-items-center">
                <h2>Портфолио</h2>
                <div class="d-flex portfolio">
                    <div class="portfolio__item"></div>
                    <div class="portfolio__item"></div>
                    <div class="portfolio__item"></div>
                </div>
            </div>
    </div>
</template>

<style scoped>
    .portfolio {
        flex-wrap: wrap;
    }

    .questionnaire {
        flex-wrap: wrap;
    }

    p {
        max-width: 400px;
        margin-right: 30px;
    }

    .value-know {
        font-size: 14px;
    }

    .tehnology {
        font-size: 26px;
        width: 300px;
    }

    @media screen and (max-width: 991px) {
        .portfolio {
            justify-content: center;
        }
    }

    .title {
        width: 110px;
    }

    .back-link {
        display: inline-block;
        color: cadetblue;
        text-decoration: none;
        margin-bottom: 20px;
    }

    .back-link:hover {
        color: darkblue;
    }

    .portfolio__item {
        width: 220px;
        height: 250px;
        background-color: rgb(83, 83, 83);
        margin: 20px;
    }
</style>