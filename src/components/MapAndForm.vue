<template>
    <section>
        <div class="container">
            <div class="content">

                <div class="col">
                    <iframe class="gmap_canvas" src="https://maps.google.com/maps?q=Storey%20Ave,%20san&t=&z=15&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0">
                    </iframe>
                </div>

                <div class="col s">
                    <div class="logo">
                        <img src="../assets/img/35.png" alt="">
                    </div> 

                    <h4>9840 Shore St. Fond DU Lac, WI 54935</h4>

                    <div class="subtext">
                        <span>0 1223 456 789</span>
                        <span>mail@sofbox.com</span>
                    </div>   

                    <div class="icons">
                        <div class="icon-box"><a href="#"><i class="fa-brands fa-facebook-f"></i></a></div>
                        <div class="icon-box"><a href="#"><i class="fa-brands fa-twitter"></i></a></div>
                        <div class="icon-box"><a href="#"><i class="fa-brands fa-github"></i></a></div>
                        <div class="icon-box"><a href="#"><i class="fa-brands fa-instagram"></i></a></div>
                    </div>

                    <h3>Get in Touch</h3>

                    <div class="form">
                        <div class="user-detail">
                            <input type="text" placeholder="Your Name" class="u_name">
                            <input type="text" placeholder="Your Email" class="u_email">
                        </div>

                        <div class="subject">
                            <input type="text" placeholder="Your Subject" class="u_subject">
                        </div>

                        <textarea name="message" cols="60" rows="10" placeholder="Your Message"></textarea>

                        <div class="btn">
                            <a href="#">Send Message</a>
                        </div>
                    </div>


                </div>

            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'MapAndForm',
}
</script>
<style lang="scss" scoped>
@import '../style/vars.scss';
@import '../style/btn.scss';

    .content {
        display: flex;
        justify-content: space-between;
        .col {
        width: calc(100% / 2);
            iframe {
                width: 100%;
                height: 500px;
            }
            .logo {
                width: 120px;
            }

            h4 {
                margin-top: 50px;
                font-size: 19px;
            }

            .subtext {
                margin: 20px 0;
                span {
                    margin: 10px 0;
                    display: block;
                    color: $sub_text;
                }
            }

            .icons {
                display: flex;
                margin: 50px 0;
                .icon-box {
                    height: 38px;
                    width: 38px;
                    margin-right: 10px;
                    box-shadow: rgba(0, 0, 0, 0) 0px 1px 3px 0px, rgba(151, 151, 151, 0.15) 0px 0px 0px 1px;
                    text-align: center;
                    line-height: 38px;
                    color: $main_color;
                }
            }
               

            h3 {
                margin: 20px 0;
                font-size: 23px;
            }

            .form {
                input, textarea {
                    border: none;
                    box-shadow: rgba(0, 0, 0, 0) 0px 1px 3px 0px, rgba(151, 151, 151, 0.15) 0px 0px 0px 1px;
                    font-family: Arial; color: #333;
                    padding: 10px;
                    margin: 10px 0;
                }

                .user-detail {
                    display: flex;
                    justify-content: space-between;
                    input {
                        width: calc(100% / 2 - 15px);
                    }
                }

                .subject {
                    input {
                        width: 100%;
                    }
                }

                textarea {
                    width: 100%;
                }

                .btn {
                    margin: 20px 0;
                    width: 150px;
                    font-size: 14px;
                    padding: 15px 0;
                }
            }
        }

        .s {
            margin-left: 20px;
        }
    }

</style>