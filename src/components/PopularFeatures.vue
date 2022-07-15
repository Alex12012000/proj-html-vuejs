<template>
    <section>
        <img src="../assets/img/14.png" alt="" class="detail">
        <div class="container">
            <div class="features-header">
                <div class="main-text">
                    <h2>Popular features that your business needs</h2>
                    <p>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot fanny!</p>
                </div>
                <div class="btn">
                    <a href="#">Explore More Feature</a>
                </div>
            </div>
            <div class="cards">
                <div class="col">
                    <div class="card">
                        <h3>Customized Invoices</h3>
                        <i class="fa-solid fa-chart-column blue"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Stock Management</h3>
                        <i class="fa fa-paper-plane orange"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Receivable & Payables</h3>
                        <i class="fa-solid fa-comments-dollar aqua"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Manage Buying</h3>
                        <i class="fa-solid fa-people-roof blue"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Powerful & Secure</h3>
                        <i class="fa-brands fa-superpowers orange"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Fastest Return Filing</h3>
                        <i class="fa-solid fa-comments-dollar aqua"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Monthly Detailed</h3>
                        <i class="fa-solid fa-file-invoice blue"></i>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <h3>Product Management</h3>
                        <i class="fa-solid fa-boxes-packing orange"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'PopularFeatures'
}
</script>
<style lang="scss" scoped>
@import '../style/btn.scss';
@import '../style/vars.scss';
    .features-header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        .main-text {
            width: 70%;
            p {
                margin: 20px 0;
            }
        }
        .btn {
           padding: 15px 30px;
        }
    }

    .cards {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }

    .col {
        width: calc(100% / 4 - 15px);
        padding: 20px;
        border-radius: 4px;
        margin: 10px 0;
        box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;

        .card {
            h3 {
                font-size: 16px;
            }
            i {
                font-size: 40px;
                margin: 25px 0;
                align-content: center;
            }

            .blue {
                color: $main_color;
            }

            .orange {
                color: $orange;
            }

            .aqua {
                color: $aqua;
            }
        }
    }


    section {
        position: relative;
        .detail {
            position: absolute;
            top: -100px;
            left: -385px;
            width: 600px;
        }
    }

</style>