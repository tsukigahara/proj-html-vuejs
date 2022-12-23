<script>
export default {

}
</script>

<template>
    <section id="home" style="background-image: url(../src/assets/img/bg-6.jpg)">
        <!-- container -->
        <div class="container d-flex justify-content-md-end justify-content-center">
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
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#home {
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 800px;
    height: 100%;
    display: flex;
    justify-content: center;

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