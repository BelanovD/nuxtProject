<template>
    <section>
        <h1>Анкеты специалистов</h1>
        <div class="d-flex questionnaire">
            <div class="flex-left">
                <div class="applicant-photo">
                    <!-- <img src="" alt="{}"> -->
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
                    <p class="title"><b>О себе:</b></p>
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
                <div class="tehnology-block d-flex justify-content-between mt-auto">
                    <div class="d-flex justify-content-between tehnology">
                        <p>HTML</p>
                        <p>CSS</p>
                        <p>JS</p>
                    </div>
                    <div class="right"><a href="/applicants_user" class="btn btn-primary">Подробнее</a></div>
                </div>
            </div>
        </div>
        <hr>
    </section>
</template>

<style scoped>
    .tehnology-block {
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

    .title {
        width: 90px;
    }

    hr {
        max-width: 850px;
    }
</style>