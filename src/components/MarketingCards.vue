<template>
    <section>
        <div class="container cards">
            <div class="col">
                <div class="card">
                    <div class="main-content">
                        <!-- icon -->
                        <img src="../assets/img/24.png" alt="">
                        <!-- all text -->
                        <div class="card-text">
                            <h3>Online Marketing</h3>
                            <p>It is along established fact that a reader will be distracted.</p>
                        </div>
                    </div>
                    <div class="benefits-list">
                        <ul>
                            <li><i class="fa-solid fa-check"></i>SEO</li>
                            <li><i class="fa-solid fa-check"></i>SEM</li>
                            <li><i class="fa-solid fa-check"></i>Website Strategy</li>
                            <li><i class="fa-solid fa-check"></i>Social management</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card">
                    <div class="main-content">
                        <!-- icon -->
                        <img src="../assets/img/24.png" alt="">
                        <!-- all text -->
                        <div class="card-text">
                            <h3>Online Marketing</h3>
                            <p>It is along established fact that a reader will be distracted.</p>
                        </div>
                    </div>
                     <div class="benefits-list">
                        <ul>
                            <li><i class="fa-solid fa-check"></i>SEO</li>
                            <li><i class="fa-solid fa-check"></i>SEM</li>
                            <li><i class="fa-solid fa-check"></i>Website Strategy</li>
                            <li><i class="fa-solid fa-check"></i>Social management</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card">
                    <div class="main-content">
                        <!-- icon -->
                        <img src="../assets/img/24.png" alt="">
                        <!-- all text -->
                        <div class="card-text">
                            <h3>Online Marketing</h3>
                            <p>It is along established fact that a reader will be distracted.</p>
                        </div>
                    </div>
                     <div class="benefits-list">
                        <ul>
                            <li><i class="fa-solid fa-check"></i>SEO</li>
                            <li><i class="fa-solid fa-check"></i>SEM</li>
                            <li><i class="fa-solid fa-check"></i>Website Strategy</li>
                            <li><i class="fa-solid fa-check"></i>Social management</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'MarketingCards'
}
</script>
<style lang="scss" scoped>
@import '../style/vars.scss';

    .cards {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .col {
        width: calc(100% / 3);
        .card {
            .main-content {
                display: flex;
                align-items: center;

                img {
                    width: 80px;
                    margin-right:20px;
                }

               .card-text {
                    h3 {
                        font-size: 20px;
                    }

                    p {
                        margin: 10px 0;
                        color: $sub_text;
                    }
                }
            }
        }

        .benefits-list {
            display: flex;
            justify-content: center;
            ul {
                padding-left: 50px;
                li {
                    list-style-type: none;
                    margin: 15px 0;
                    font-weight: 600;
                    font-size: 14px;
                    i {
                        margin-right: 15px;
                        color: $main_color;
                    }
                }
            }
        }
    }
</style>