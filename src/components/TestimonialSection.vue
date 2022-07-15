<template>
    <section>
        <div class="container">

            <!-- header text-->
            <div class="header">
                <h2>Our Testimonials</h2>
                <p>If you are planning on developing a product landing app or website, take a look at this beautiful-crafted</p>
            </div>

            <!-- testimonial cards -->
            <div class="testimonial">
                <div class="col">
                <div class="card">
                    <div class="user-img">
                        <img src="../assets/img/26.jpeg" alt="">
                    </div>
                    <div class="name">
                        <h3>Julia Aann</h3>
                        <span>- COO Sofbox</span>
                    </div>
                    <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>

                    <div class="bg-quote">
                        <img src="../assets/img/quotes.png" alt="">
                    </div>
                </div>

                <div class="under-card"></div>
                <div class="under-card short"></div>
                
            </div>
            <div class="col">
                <div class="card">
                    <div class="user-img">
                        <img src="../assets/img/27.jpeg" alt="avatar">
                    </div>
                    <div class="name">
                        <h3>Mac Znder</h3>
                        <span>- Manager Sofbox</span>
                    </div>
                    <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip.</p>

                    <div class="bg-quote">
                        <img src="../assets/img/quotes.png" alt="avatar">
                    </div>
                </div>

                <div class="under-card"></div>
                <div class="under-card short"></div>
            </div>
            </div>
            
            <!-- switch -->
            <div class="switch">
                <div class="dot"></div>
                <div class="dot"></div>
            </div>

        </div>
    </section>
</template>
<script>
export default {
    name: 'TestimonialSection'    
}
</script>
<style lang="scss" scoped>
@import '../style/vars.scss';

    section {
        background-image: url('../assets/img/15.png') , linear-gradient(180deg, rgba(242,247,255,1) 43%, rgba(255,255,255,1) 100%);
        background-repeat: no-repeat;
        background-size: contain;
        background-position-y: -50px;
    }

    .header {
        width: 60%;
        margin: 0 auto;
        text-align: center;
        margin-bottom: 90px;
        
        p {
            margin: 20px 0;
        }

    }

    .testimonial {
        display: flex;
        justify-content: space-between;
        position: relative;

        .col {
            width: calc((100% / 2) - 30px); 
            position: relative;
            z-index: 10;
            .card {
                width: 100%;
                background-color: white;
                box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
                padding: 25px;
                position: relative;
                z-index: 10;

                .user-img {
                    display: flex;
                    justify-content: center;
                    img {
                        margin: 20px 0;
                        overflow: hidden;
                        width: 80px;
                        border-radius: 50%;
                    }
                }

                .name {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    margin-bottom: 30px;
                    span {
                        color: $sub_text;
                        margin-left: 5px;
                    }
                }

                p {
                    margin-bottom: 20px;
                }

                .bg-quote {
                    width: 150px;
                    filter: opacity(6%);
                    position: absolute; 
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -20%);
                }   
            }

            .under-card {
                width: 90%;
                height: 290px;
                background-color: white;
                box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -45%);
                z-index: 2;
            }

            .short {
                width: 80%;
                height: 310px;
                z-index: 1;
            }
            
        }
        
    }

    .switch {
        margin: 70px 0;
        display: flex;
        justify-content: center;
        .dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: black;
            margin: 0 5px;
        }

        .dot:first-child {
            background-color: $main_color;
        } 
    }
    
</style>