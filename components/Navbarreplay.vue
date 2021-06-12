<template>
    <header>
        <div class="container-fluid">
            <nuxt-link exect class="navbar-brand" to="/">IT manager</nuxt-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
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
                        <nuxt-link active-class="active" class="nav-link" to="/services">Услуги</nuxt-link>
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
                    <li class="nav-item dropdown">
                        <nuxt-link class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        Dropdown
                        </nuxt-link>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><nuxt-link class="dropdown-item" href="#">Action</nuxt-link></li>
                            <li><nuxt-link class="dropdown-item" href="#">Another action</nuxt-link></li>
                            <li><hr class="dropdown-divider"></li>
                            <li><nuxt-link class="dropdown-item" href="#">Something else here</nuxt-link></li>
                        </ul>
                    </li>
                    <li class="nav-item">
                    <nuxt-link class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</nuxt-link>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>