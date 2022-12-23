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
                    <small>our editorial content</small>
                    <h2>latest <span class="word">news</span></h2>
                    <!-- content -->
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat, culpa laborum.
                    </p>
                </div>
                <!-- see more button -->
                <button type="button" class="btn my_btn">SEE ALL</button>
            </div>
            <!-- cards bootstrap -->
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-4 my-2">
                <a href="">
                    <div class="col">
                        <div class="card">
                            <img src="../assets/img/news-1.jpg" class="card-img" alt="...">
                            <div class="card-img-overlay">
                                <h5 class="card-title">Card title</h5>
                                <p class="card-text"><small>Last updated 3 mins ago</small></p>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="">
                    <div class="col">
                        <div class="card">
                            <img src="../assets/img/news-1.jpg" class="card-img" alt="...">
                            <div class="card-img-overlay">
                                <h5 class="card-title">Card title</h5>
                                <p class="card-text"><small>Last updated 3 mins ago</small></p>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="">
                    <div class="col">
                        <div class="card">
                            <img src="../assets/img/news-1.jpg" class="card-img" alt="...">
                            <div class="card-img-overlay">
                                <h5 class="card-title">Card title</h5>
                                <p class="card-text"><small>Last updated 3 mins ago</small></p>
                            </div>
                        </div>
                    </div>
                </a>

            </div>
        </div>
        <!-- container end -->
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#news {
    background-color: white;
    color: $shark;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            display: flex;
            justify-content: space-between;
            flex-flow: row wrap;

            button {
                align-self: flex-end;
            }
        }

        .card-img-overlay {
            display: flex;
            flex-flow: column;
            align-items: center;
            justify-content: end;
            background-color: rgba(0, 0, 0, 0.405);

            &:hover {
                background-color: $word;
            }

            .card-title {
                color: white;
                font-size: 24px;
                font-weight: 600;
            }
        }


    }

}
</style>