<template>
    <div class="big-container jumbo">
        <div class="jumbo-content">
            <!-- Main Text -->
            <h1>The biggest platform for your growth.</h1>
            <p>There are many variations of passages of Lorem lpsum available, but the majority have suffered alteration in some form</p>

            <!-- CTA button -->
            <div class="btn">
                <a href="#">Read More</a>
            </div>
        </div>

        <!-- Big Img -->
        <div class="jumbo-img">
            <img src="../assets/img/27-1.png" alt="">
        </div>
    </div>
</template>
<script>
export default {
   name: 'PageJumbotron' 
}
</script>
<style lang="scss" scoped>
@import '../style/btn.scss';
@import '../style/vars.scss';

.jumbo {
    display: flex;
    position: relative;
    background-color: $second_color;
    padding: 40px;
    border-radius: 10px;

    .jumbo-content {
        width: calc((100% / 2) - 50px);

        h1 {
            font-size: 43px;
            line-height: 60px;
            word-spacing: 5px;
            margin: 20px 0;
        }

        p {
            font-size: 15px;
            color: $sub_text;
            margin: 20px 0;
        }

        .btn {
            width: 120px;
            margin: 60px 0;
        }
    }

    .jumbo-img {
        position: absolute;
        top: 20px;
        right: 0;
    }
}
    
</style>