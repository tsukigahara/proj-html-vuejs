<script>
// fontawesome////////
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

export default {
    components: {
        FontAwesomeIcon,
    },
    props: {
        list: Array,
    },
    data() {
        return {
            icolor: '#45bbbc',
            newList: []

        }
    },
    methods: {
        filterArray() {
            this.$props.list.forEach(element => {
                if (element.drop == true) {
                    this.newList.push(element)
                }
                else {
                    return
                }
                console.log(this.newList)
            });

        }
    },
    // è corretto?
    mounted() {
        this.filterArray()
    },
}
</script>

<template>
    <footer id="footer">
        <!-- container -->
        <div class="container">
            <!-- wrapper -->
            <div class="row">
                <div class="col-lg-3 col-12">
                    <div class="infobox">
                        <!-- logo -->
                        <a href="">
                            <img src="../assets/img/nexgen-logo.svg" class="mb-3" alt="logo" width="150">
                        </a>
                        <p>
                            A functional HTML Template for Corporate & Business
                        </p>
                        <p>
                            phone number
                        </p>
                        <p>
                            email
                        </p>
                        <p>
                            adress
                        </p>
                        <a href="#home" type="button" class="btn my_btn">GET IN TOUCH</a>
                    </div>
                </div>
                <div class="col-3 d-none d-lg-block" v-for="(item, index) in newList" :key="index">
                    <div class="linkbox">
                        <h3>{{ item.name }}</h3>
                        <ul class="">
                            <li class="" v-for="(subitem, index) in item.subitems" :key="index">
                                <a :href="subitem.url">
                                    <span><font-awesome-icon icon="fa-solid fa-angle-right" fixed-width /></span>
                                    {{ subitem.name }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <section class="credit">
                <small>©️ 2020 NEXGEN is made with love by <a href="">Tsukigahara</a></small>
            </section>
        </div>
        <!-- container end -->
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#footer {
    background-color: $woodsmoke;
    color: white;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;

        .linkbox {
            height: 100%;
            background-color: rgba(59, 59, 59, 0.253);
            padding: 2rem;
            border-radius: 10px;

            h3 {
                color: white;
            }

            ul {
                color: gray;

                li {
                    margin-bottom: 0.5rem;

                    a {
                        // for next line indent
                        display: flex;
                    }
                }
            }
        }

        .credit {
            padding: 3rem 0;

            small {
                color: gray;

                a {
                    color: $fountainblue;
                }

            }
        }
    }


}
</style>