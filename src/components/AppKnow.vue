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
    <section id="know" style="background-image: url(../src/assets/img/bg-1.jpg)">
        <!-- container -->
        <div class="container d-flex justify-content-center flex-column flex-md-row">
            <!-- wrapper -->
            <div class="infobox">
                <!-- title -->
                <small>newsletter</small>
                <h2><span class="word onblack">know</span> first</h2>
                <!-- content -->
                <p>
                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Exercitationem, quidem laudantium hic
                </p>
            </div>
            <!-- input div -->
            <div class="inputbox">
                <!-- form -->
                <form action="">
                    <input type="text" placeholder="Name">
                    <input type="text" placeholder="Email">
                    <button type="submit" class="btn my_btn">SUBSCRIBE</button>
                </form>
            </div>
        </div>
        <!-- container end -->
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partial/variables' as *;

#know {
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
    padding: 10% 0;

    .container {
        min-height: 100%;
        flex-flow: wrap;


        .infobox {
            flex-basis: 50%;
        }
    }

}
</style>