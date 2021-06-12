<template>
    <section>
        <form @submit.prevent="onSubmit">
            <div class="mb-3">
                <label for="emailLogin" class="form-label">Ваш E-mail</label>
                <input type="email" class="form-control" id="emailLogin" aria-describedby="emailHelp" placeholder="Введите Ваш mail...">
            </div>
            <div class="mb-3">
                <label for="passwordLogin" class="form-label">Ваш пароль</label>
                <input type="password" class="form-control" id="passwordLogin" placeholder="Введите Ваш пароль...">
            </div>
            <div class="mb-3 form-check">
                <input type="checkbox" class="form-check-input" id="exampleCheck1">
                <label class="form-check-label" for="exampleCheck1">Запомнить меня</label>
            </div>
            <button type="submit" class="btn btn-primary">Отправить</button>
        </form>
    </section>
</template>

<script>
export default {
    layout: 'empty',
    methods: {
        onSubmit() {
            this.$store.dispatch('login')
            this.$router.push('/applicants')
        }
    }
}
</script>

<style scoped>
    form {
        width: 400px;
    }

    @media screen and (max-width: 450px) {
        form {
        width: 300px;
    }
    }

    @media screen and (max-width: 350px) {
        form {
        width: 250px;
    }
    }
</style>