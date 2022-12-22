<script>
export default {
    props: {
        data: Array
    }
}
</script>

<template>
    <header>
        <section class="banner">
        </section>
        <nav class="navbar navbar-expand-lg fixed-top my_nav">
            <div class="container">
                <a class="" href="">
                    <img src="../assets/img/nexgen-logo.svg" alt="logo" width="100">
                </a>
                <!-- button for mobile -->
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                    data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false"
                    aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <!-- nav content -->
                <div class="collapse navbar-collapse justify-content-end " id="navbarNavDropdown">
                    <ul class="navbar-nav my_navbar-nav align-items-center">
                        <li class="nav-item" v-for="(item, index) in data" :key="index"
                            :class="item.drop == true ? 'dropdown' : ''">
                            <!-- without subitem -->

                            <a class="nav-link my_nav-link active" aria-current="page" :href="item.url"
                                v-if="!item.drop">{{
                                        item.name
                                }}</a>

                            <!-- with subitem (dropdown)-->
                            <a class="nav-link my_nav-link active" :href="item.url" role="button"
                                data-bs-toggle="dropdown" aria-expanded="false" v-if="item.drop">
                                {{ item.name }}
                            </a>
                            <ul class="dropdown-menu my_dropdown-menu" v-if="item.drop">
                                <li v-for="(subitem, index) in item.subitem" :key="index">
                                    <a class="dropdown-item" :href="subitem.url">{{ subitem.name }}</a>
                                </li>
                            </ul>
                        </li>
                        <li>
                            <button type="button" class="btn my_btn">GET IN TOUCH</button>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;





.my_nav {
    font-weight: 400;
    color: $shark;

    .my_navbar-nav {
        gap: 10px;
    }

    .my_nav-link {
        text-transform: uppercase;
        font-size: 14px;

        &:hover {
            color: $elm;
        }
    }

    .my_dropdown-menu {
        background-color: rgba(220, 220, 220, 0.872);
    }
}
</style>
