<template>
    <section>
        <div class="container">
            <!-- Section Header -->
            <div class="section-header">
                <h2>Latest Post</h2>
                <span>If you are planning on developing a product landing.</span>
            </div>
            <!-- Cards -->
            <div class="cards">
                <div class="col">
                    <div class="card">
                        <img src="../assets/img/19.jpg" alt="">
                        <h3>Life Lack Meaning</h3>
                        <p>It is a long established fact that a reader will be distracted by the readable.</p>
                    </div>
                    <div class="tag">
                        <span>November 28, 2019</span>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <img src="../assets/img/18.jpg" alt="">
                        <h3>Life Lack Meaning</h3>
                        <p>It is a long established fact that a reader will be distracted by the readable.</p>
                    </div>
                    <div class="tag">
                        <span>November 28, 2019</span>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <img src="../assets/img/17.jpg" alt="">
                        <h3>Life Lack Meaning</h3>
                        <p>It is a long established fact that a reader will be distracted by the readable.</p>
                    </div>
                    <div class="tag">
                        <span>November 28, 2019</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'LastPosts'
}
</script>
<style lang="scss" scoped>
@import '../style/vars.scss';

    .section-header {
        text-align: center;
        margin-bottom: 80px;
        h2 {
            margin: 10px 0;
        }
        span {
            color: $sub_text;
        }
    }

    .cards {
        display: flex;
        justify-content: space-between;
        .col {
            width: calc((100% / 3) - 15px);
            position: relative;
            .card {
                padding: 10px;
                box-shadow: rgba(0, 0, 0, 0.05) 0px 0px 0px 1px;
                h3 {
                    margin: 20px 0;
                }
                p {
                    padding-right: 30px;
                    margin-bottom: 10px;
                    line-height: 25px;
                }
            }

            .tag {
                position: absolute;
                top: 15px;
                left: 15px;
                padding: 7px;
                border-radius: 5px;
                background-color: white;
                font-size: 13px;
                color: $sub_text;
            }

            .tag:hover {
                color: $main_color;
            }
        }
    }
    
</style>