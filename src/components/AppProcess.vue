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
    <section id="process">
        <!-- container -->
        <div class="container-fluid d-flex justify-content-center align-items-center flex-column">
            <!-- wrapper flex-->
            <div class="infobox">
                <!-- title -->
                <small>how it works in practice</small>
                <h2><span class="word">process</span> management</h2>
                <!-- content -->
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat, culpa laborum. Ipsum quidem,
                    maxime sunt, consequatur ipsa, dolores tempore ratione
                </p>
            </div>
            <div class="timeline">
                <!-- line for lg device -->
                <span class="h-line d-none d-lg-block"></span>
                <!-- live for sm device -->
                <span class="v-line d-block d-lg-none"></span>
                <!-- card group -->
                <div class="row row-cols-1 row-cols-lg-5 g-4 my_card-group">
                    <!-- card -->
                    <div class="col">
                        <div class="card border- py-3">
                            <div class="card-body text-center">
                                <!-- number title -->
                                <div class="title_number">01</div>
                                <!-- title -->
                                <h5 class="card-title">Collection of information</h5>
                                <!-- content -->
                                <p class="card-text">
                                    This is a longer card with supporting text
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card py-3">
                            <div class="card-body text-center">
                                <!-- number title -->
                                <div class="title_number">02</div>
                                <!-- title -->
                                <h5 class="card-title">Collection of information</h5>
                                <!-- content -->
                                <p class="card-text">
                                    This is a longer card with supporting text
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card py-3">
                            <div class="card-body text-center">
                                <!-- number title -->
                                <div class="title_number">03</div>
                                <!-- title -->
                                <h5 class="card-title">Collection of information</h5>
                                <!-- content -->
                                <p class="card-text">
                                    This is a longer card with supporting text
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card py-3">
                            <div class="card-body text-center">
                                <!-- number title -->
                                <div class="title_number">04</div>
                                <!-- title -->
                                <h5 class="card-title">Collection of information</h5>
                                <!-- content -->
                                <p class="card-text">
                                    This is a longer card with supporting text
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card py-3">
                            <div class="card-body text-center">
                                <!-- number title -->
                                <div class="title_number">05</div>
                                <!-- title -->
                                <h5 class="card-title">Collection of information</h5>
                                <!-- content -->
                                <p class="card-text">
                                    This is a longer card with supporting text
                                </p>
                            </div>
                        </div>
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

#process {
    background-color: white;
    color: $shark;
    padding: 10% 0;

    .container-fluid {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            width: 60%;
            display: flex;
            flex-flow: column;
            justify-content: center;
            align-items: center;
        }

        .timeline {
            width: 100%;
            margin-top: 30px;
            display: flex;
            flex-flow: column;
            align-items: center;
            justify-content: center;
            position: relative;


            .h-line {
                width: 100%;
                border-top: 5px solid $line;
            }

            .v-line {
                position: absolute;
                top: -30px;
                height: 800px;
                border-left: 5px solid $line;

            }

            .my_card-group {
                width: 90%;

                .title_number {
                    width: 40px;
                    height: 40px;
                    line-height: 40px;
                    text-align: center;
                    background-color: $line;
                    color: $bluelagoon;
                    border-radius: 100%;
                    position: absolute;
                    top: -20px;
                    left: 50%;
                    translate: -50% 0%;
                }

                .card {
                    border: 5px solid $line
                }

                // for small device card layout
                @media only screen and (min-width : 992px) {
                    .card {
                        border: 0;
                    }
                }
            }
        }
    }


}
</style>