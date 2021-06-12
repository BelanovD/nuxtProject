<template>
    <header>
        <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
            <div class="container-fluid">
                <nuxt-link exect class="navbar-brand" to="/">IT manager</nuxt-link>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <nuxt-link active-class="active" class="nav-link" to="/employers">Работодателям</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link active-class="active" class="nav-link" to="/applicants">Соискателям</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link active-class="active" class="nav-link" to="/contacts">Контакты</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link active-class="active" class="nav-link" to="/login">Login</nuxt-link>
                        </li>
                        <li class="nav-item" v-if="isAuth">
                            <a class="nav-link" href="#" @click.prevent="logout">Logout</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    computed: {
        isAuth() {
            return this.$store.getters.isAuth
        }
    },
    methods: {
        logout() {
            this.$store.dispatch('logout')
        }
    }
}
</script>