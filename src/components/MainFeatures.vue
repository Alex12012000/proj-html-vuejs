<template >
    <section>
        <div class="container main-features">
            <div class="main-features-content">
                <div class="main-text">
                    <h2>Get tips tricks on how to skyrocket your sales.</h2>
                    <p>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny!</p>
                </div>
                <div class="cards">
                    <div class="card ">
                        <img src="../assets/img/510.png" alt="">
                        <div class="card-text">
                            <h3>
                             Reporting Analysis
                            </h3>
                            <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
                        </div>
                    </div>
                    <div class="card ">
                        <img src="../assets/img/511.png" alt="">
                        <div class="card-text">
                            <h3>
                             Reporting Analysis
                            </h3>
                            <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="main-features-img">
                <img src="../assets/img/509.jpeg" alt="">
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'MainFeatures'
}
</script>
<style lang="scss" scoped>
@import '../style/vars.scss';

    .main-features {
        display: flex;
        justify-content: space-between;
        .main-features-content {
            width: calc((100% / 2) - 30px);
            .main-text {
                margin-bottom: 50px;
                p {
                    margin: 20px 0;
                }
            }
            p {
                margin: 10px 0;
                font-size: 13px;
            }
            .card {
                display: flex;
                align-items: center;
                padding: 10px;
                margin: 15px 0;
                img {
                    width: 60px;
                    height: 60px;
                    margin-right: 20px;
                }
            }

            .card:first-child {
                box-shadow: 0 21px 38px rgba(0,0,0,0.08), 0 15px 12px rgba(0,0,0,0.08);
            }
        }

        .main-features-img {
            width: calc((100% / 2) - 10px);
        }
        
    }
</style>