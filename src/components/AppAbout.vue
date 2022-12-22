<script>
// fontawesome////////
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

export default {
    components: {
        FontAwesomeIcon,
    },
    data() {
        return {
            icolor: '#45bbbc',

        }
    },
}
</script>

<template>
    <section id="about">
        <!-- container -->
        <div class="container d-flex justify-content-center flex-column flex-md-row">
            <!-- wrapper -->
            <div class="infobox">
                <!-- title -->
                <small>about the network</small>
                <h2><span class="word onblack">The</span> company</h2>
                <!-- content -->
                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Exercitationem, quidem laudantium hic
                </p>
                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Exercitationem, quidem laudantium hic
                </p>
            </div>
            <!-- cards -->
            <div class="cardbox">
                <!-- card -->
                <div class="card my_card" style="width: 15rem;">
                    <div class="card-body">
                        <!-- title -->
                        <h5 class="card-title">
                            <span>
                                <font-awesome-icon icon="fa-solid fa-medal" :color="icolor" />
                            </span>
                            Tradition
                        </h5>
                        <!-- content -->
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        </p>
                    </div>
                </div>
                <!-- card -->
                <div class="card my_card" style="width: 15rem;">
                    <div class="card-body">
                        <!-- title -->
                        <h5 class="card-title">
                            <span>
                                <font-awesome-icon icon="fa-solid fa-lock" :color="icolor" />
                            </span>
                            Security
                        </h5>
                        <!-- content -->
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        </p>
                    </div>
                </div>
                <!-- card -->
                <div class="card my_card" style="width: 15rem;">
                    <div class="card-body">
                        <!-- title -->
                        <h5 class="card-title">
                            <span>
                                <font-awesome-icon icon="fa-solid fa-pen-to-square" :color="icolor" />
                            </span>
                            Certificate
                        </h5>
                        <!-- content -->
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        </p>
                    </div>
                </div>
                <!-- card -->
                <div class="card my_card" style="width: 15rem;">
                    <div class="card-body">
                        <!-- title -->
                        <h5 class="card-title">
                            <span>
                                <font-awesome-icon icon="fa-solid fa-graduation-cap" :color="icolor" />
                            </span>
                            Expertise
                        </h5>
                        <!-- content -->
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        </p>
                    </div>
                </div>
            </div>
            <!-- cards end -->
        </div>
        <!-- container end -->
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#about {
    background-color: $woodsmoke;
    color: white;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            flex-basis: 45%;
        }

        .cardbox {
            flex-basis: 55%;
            display: flex;
            flex-flow: row wrap;
            justify-content: center;
            gap: 10px;

            .my_card {
                background-color: transparent;
            }
        }
    }

}
</style>