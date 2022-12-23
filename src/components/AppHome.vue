<script>
export default {

}
</script>

<template>
    <section id="home" style="background-image: url(../src/assets/img/bg-6.jpg)">
        <div class="bg_overlay">
            <!-- container -->
            <div class="container d-flex justify-content-lg-end justify-content-center">
                <!-- wrapper -->
                <div class="my_wrapper">
                    <!-- titles -->
                    <small>fusion & acquisitions</small>
                    <h1>insurance consulting</h1>
                    <!-- form -->
                    <form>
                        <!-- input group -->
                        <div class="row row-cols-1 row-cols-lg-2 g-3">
                            <div class="col">
                                <input class="" type="text" placeholder="Name">
                            </div>
                            <div class="col">
                                <input class="" type="text" placeholder="Email">
                            </div>
                            <div class="col">
                                <input class="" type="text" placeholder="Phone">
                            </div>
                            <div class="col">
                                <select name="" id="">
                                    <option selected>More Info</option>
                                    <option value="">lorem</option>
                                    <option value="">lorem</option>
                                    <option value="">lorem</option>
                                </select>
                            </div>
                            <!-- buttons -->
                            <div class="col">
                                <button class="btn my_btn" type="submit">GET IN TOUCH</button>
                            </div>
                            <div class="col">
                                <a class="btn my_btn_border" href="#about">READ MORE</a>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#home {
    background-repeat: no-repeat;
    background-size: cover;

    // backgroud overlay for black opacity
    .bg_overlay {
        width: 100%;
        height: 100%;
        padding: 20% 0;
        transition: 3s;

        // background opacity when witdh < 992px
        @media only screen and (max-width : 992px) {
            & {
                background-color: rgba(0, 0, 0, 0.608);
                transition: 3s;
            }

            // change h1 color 
            .my_wrapper {
                h1 {
                    color: white;
                }

            }
        }
    }

    .my_wrapper {
        display: flex;
        flex-flow: column;
        justify-content: center;
        max-width: 400px;

        small {
            font-size: 14px;
            font-weight: 500;
            text-transform: uppercase;
        }

        h1 {
            font-size: 48px;
            font-weight: 800;
            color: $shark;
            text-transform: capitalize;
        }

        form {

            input {
                margin: 0;
            }

            select {
                min-height: 40px;
                width: 100%;
                border: 0;
                border-radius: 5px;
                color: gray;
                padding: 10px;
                background-color: rgba(218, 218, 218, 0.92);
            }

            .btn {
                width: 100%
            }
        }
    }

}
</style>