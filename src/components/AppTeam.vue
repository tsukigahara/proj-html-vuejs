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
    <section id="team">
        <!-- container -->
        <div class="container d-flex justify-content-start flex-lg-row flex-column">
            <!-- wrapper -->
            <div class="infobox">
                <div>
                    <!-- title -->
                    <small>we like what we do</small>
                    <h2><span class="word onblack">Team</span> of experts</h2>
                    <!-- content -->
                    <p>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Exercitationem, quidem laudantium hic
                    </p>
                </div>
                <!-- cards -->
                <div class="row row-cols-1 row-cols-sm-2 g-2 mt-3">
                    <!-- card -->
                    <div class="col">
                        <div class="card mt-3">
                            <div class="row g-0">
                                <div class="col-md-4">
                                    <img src="../assets/img/team-1.jpg" class="img-fluid rounded" alt="...">
                                </div>
                                <div class="col-md-8">
                                    <div class="card-body">
                                        <h5 class="card-title">John Appleseed</h5>
                                        <p class="card-text">CEO & FOUNDER</p>
                                        <p class="card-text"><button type="button"
                                                class="btn btn-primary">Button</button>
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card mt-3">
                            <div class="row g-0">
                                <div class="col-md-4">
                                    <img src="../assets/img/team-1.jpg" class="img-fluid rounded" alt="...">
                                </div>
                                <div class="col-md-8">
                                    <div class="card-body">
                                        <h5 class="card-title">John Appleseed</h5>
                                        <p class="card-text">CEO & FOUNDER</p>
                                        <p class="card-text"><button type="button"
                                                class="btn btn-primary">Button</button>
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card mt-3">
                            <div class="row g-0">
                                <div class="col-md-4">
                                    <img src="../assets/img/team-1.jpg" class="img-fluid rounded" alt="...">
                                </div>
                                <div class="col-md-8">
                                    <div class="card-body">
                                        <h5 class="card-title">John Appleseed</h5>
                                        <p class="card-text">CEO & FOUNDER</p>
                                        <p class="card-text"><button type="button"
                                                class="btn btn-primary">Button</button>
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="card mt-3">
                            <div class="row g-0">
                                <div class="col-md-4">
                                    <img src="../assets/img/team-1.jpg" class="img-fluid rounded" alt="...">
                                </div>
                                <div class="col-md-8">
                                    <div class="card-body">
                                        <h5 class="card-title">John Appleseed</h5>
                                        <p class="card-text">CEO & FOUNDER</p>
                                        <p class="card-text"><button type="button"
                                                class="btn btn-primary">Button</button>
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- speech card -->
            <div class="speechbox">
                <div class="card p-4">
                    <div class="card-body">
                        <h5 class="card-title mb-3">President's speech</h5>
                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                        <div class="d-flex justify-content-between"><small>JOHN APPLESEED</small>
                            <div class="dot">"</div>
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

#team {
    background-color: $woodsmoke;
    color: white;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            flex-basis: 65%;

            .card {
                background-color: transparent;
            }
        }

        .speechbox {
            flex-basis: 35%;
            display: flex;
            overflow-y: auto;

            .card {
                background-color: $bluelagoon;

                .card-title {
                    font-weight: 600;

                }

                p {
                    color: white;

                }

                .dot {
                    font-size: 70px;
                    color: $limedspruce;
                    line-height: 0.8;

                }

            }
        }

    }

}
</style>