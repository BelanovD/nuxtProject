<template>
    <section>
        <h1>Анкета специалиста</h1>
        <h2>Заполните анкету</h2>
        <form>
            <div class="mb-3">
                <label for="applicantName" class="form-label">Как Вас зовут?</label>
                <input type="text" class="form-control" id="applicantName">
            </div>
            <div class="mb-3">
                <label for="tehnology" class="form-label">Перечислите через запятую технологии, с которыми Вы знакомы (HTML, CSS, Vue и т.д.)</label>
                <input type="text" class="form-control" id="tehnology">
            </div>
            <div class="mb-3">
                <label class="form-label" for="inputGroupSelect01">Оцените от 1 до 10 свой навык владения Html</label>
                <select class="form-select" id="inputGroupSelect01">
                    <option selected>1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                    <option value="4">4</option>
                    <option value="5">5</option>
                    <option value="6">6</option>
                    <option value="7">7</option>
                    <option value="8">8</option>
                    <option value="9">9</option>
                    <option value="10">10</option>
                </select>
            </div>
            <div class="mb-3">
                <label class="form-label" for="inputGroupSelect02">Оцените от 1 до 10 свой навык владения Css</label>
                <select class="form-select" id="inputGroupSelect02">
                    <option selected>1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                    <option value="4">4</option>
                    <option value="5">5</option>
                    <option value="6">6</option>
                    <option value="7">7</option>
                    <option value="8">8</option>
                    <option value="9">9</option>
                    <option value="10">10</option>
                </select>
            </div>
            <div class="mb-3">
                <label class="form-label" for="inputGroupSelect03">Оцените от 1 до 10 свой навык владения JS</label>
                <select class="form-select" id="inputGroupSelect03">
                    <option selected>1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                    <option value="4">4</option>
                    <option value="5">5</option>
                    <option value="6">6</option>
                    <option value="7">7</option>
                    <option value="8">8</option>
                    <option value="9">9</option>
                    <option value="10">10</option>
                </select>
            </div>
            <div class="mb-3">
                <label for="hardSkills" class="form-label">Перечислите свои Hard Skills</label>
                <textarea class="form-control" id="hardSkills" rows="3"></textarea>
            </div>
            <div class="mb-3">
                <label for="softSkills" class="form-label">Перечислите свои Soft Skills</label>
                <textarea class="form-control" id="softSkills" rows="3"></textarea>
            </div>
            <div class="mb-3">
                <label for="applicantAbout" class="form-label">Напишите коротко о себе, чем увлекаетесь, а также укажите дополнительную информацию, если желаете</label>
                <textarea class="form-control" id="applicantAbout" rows="3"></textarea>
            </div>
            <div class="mb-3">
                <label for="applicantFoto" class="form-label">Загрузите фотографию</label>
                <input class="form-control" type="file" id="applicantFoto">
            </div>
            <div class="mb-3">
                <label for="portfolio" class="form-label">Ссылка на работу из портфолио</label>
                <input class="form-control" type="text" id="portfolio">
            </div>
            <div class="mb-3">
                <label for="applicantMail" class="form-label">Укажите Ваш E-mail</label>
                <input type="email" class="form-control" id="applicantMail" aria-describedby="emailHelp">
            </div>
            <button type="submit" class="btn btn-primary">Отправить</button>
    </form>
    </section>
</template>

<style scoped>
    h2 {
        margin-top: 40px;
    }
    form {
        margin-bottom: 40px;
    }
</style>

<script>