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
            isize: '2x'
        }
    },
}
</script>

<template>
    <section id="news">
        <!-- container -->
        <div class="container d-flex justify-content-center justify-content-md-start flex-column">
            <!-- wrapper flex-->
            <div class="infobox">
                <div>
                    <!-- title -->
                    <small>our business areas</small>
                    <h2>Excellence in <span class="word">Services</span></h2>
                    <!-- content -->
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat, culpa laborum. Ipsum quidem,
                        maxime sunt, consequatur ipsa, dolores tempore ratione
                    </p>
                </div>
                <!-- see more button -->
                <button type="button" class="btn my_btn">SEE ALL</button>
            </div>
            <!-- cards bootstrap -->
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-4 my-2">
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>
                <div class="col">
                    <div class="card my_card h100">
                        <a href="">
                            <div class="card-body">
                                <!-- arrow icon -->
                                <span>
                                    <font-awesome-icon icon="fa-solid fa-arrow-right" :color="icolor" :size="isize" />
                                </span>
                                <!-- title icon -->
                                <h5 class="mb-3">
                                    <font-awesome-icon icon="fa-solid fa-network-wired" :color="icolor" :size="isize" />
                                </h5>
                                <!-- title -->
                                <h5 class="my_card-title mb-3">Card title</h5>
                                <!-- content -->
                                <p class="card-text">This is a longer card with supporting text below as a natural
                                    lead-in
                                    to additional
                                    content.</p>
                            </div>
                        </a>
                    </div>
                </div>

            </div>
        </div>
        <!-- container end -->
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#news {
    background-color: $blackhaze;
    color: $shark;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            display: flex;
            justify-content: space-between;
            flex-flow: row wrap;

            div {
                flex-basis: 70%;
            }

            button {
                align-self: flex-end;
            }

        }

        .my_card {
            border: 0;

            &:hover {
                background-color: #3d49551c;
            }

            .card-body {
                padding: 1.5em 3em;
                position: relative;

                span {
                    position: absolute;
                    right: 40px;
                    top: 40px;
                }

                .my_card-title {
                    font-weight: 600;
                    font-size: 24px;
                }
            }
        }


    }

}
</style>