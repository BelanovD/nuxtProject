<template>
    <section>
        <h1>Контакты</h1>
        <div class="contacts">
            <p>info@fakeitmanger.com <br> +7-777-777-77-77 <br> ООО "АЙТИМЕНЕДЖЕР"</p>
        </div>
        <h2>Остаьте вопрос и свои контактные данные</h2>
        <form>
            <div class="mb-3">
                <label for="applicantName" class="form-label">Как к Вам обращаться?</label>
                <input type="text" class="form-control" id="applicantName">
            </div>
            <div class="mb-3">
                <label for="softSkills" class="form-label">Напишите свой вопрос</label>
                <textarea class="form-control" id="softSkills" rows="3"></textarea>
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
    .contacts {
        margin: 40px 0;
    }

    form {
        max-width: 700px;
    }
    @media screen and (max-width: 575px) {
        section {
            margin: 0 20px;
        }
    }
</style>