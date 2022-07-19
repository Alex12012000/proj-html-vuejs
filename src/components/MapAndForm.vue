<template>
    <section id="contact">
        <div class="container">
            <!-- Section Header -->
            <div class="section-header">
                <h2>Contact with our team</h2>
                <span>If you are planning on developing a product landing.</span>
            </div>
            <!-- All the content -->
            <div class="content">
                <!-- Map -->
                <div class="col">
                    <!-- Google map iframe -->
                    <iframe class="gmap_canvas" src="https://maps.google.com/maps?q=Storey%20Ave,%20san&t=&z=15&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0">
                    </iframe>
                </div>

                <!-- Content Col -->
                <div class="col small">
                    <!-- logo -->
                    <div class="logo">
                        <img src="../assets/img/35.png" alt="">
                    </div> 

                    <h4>9840 Shore St. Fond DU Lac, WI 54935</h4>

                    <!-- Contact info -->
                    <div class="subtext">
                        <span>0 1223 456 789</span>
                        <span>mail@sofbox.com</span>
                    </div>   

                    <!-- Social icons -->
                    <div class="icons">
                        <div class="icon-box"><a href="https://www.facebook.com"><i class="fa-brands fa-facebook-f"></i></a></div>
                        <div class="icon-box"><a href="https://twitter.com/"><i class="fa-brands fa-twitter"></i></a></div>
                        <div class="icon-box"><a href="https://github.com"><i class="fa-brands fa-github"></i></a></div>
                        <div class="icon-box"><a href="https://www.instagram.com/"><i class="fa-brands fa-instagram"></i></a></div>
                    </div>

                    <h3>Get in Touch</h3>

                    <!-- Form -->
                    <div class="form">

                        <div class="user-detail">
                            <input type="text" placeholder="Your Name" class="u_name" v-model="name">
                            <input type="email" placeholder="Your Email" class="u_email" v-model="email">
                        </div>

                        <div class="subject">
                            <input type="text" placeholder="Your Subject" class="u_subject" v-model="subject">
                        </div>

                        <textarea name="message" cols="60" rows="10" placeholder="Your Message" v-model="msg"></textarea>

                        <!-- Button -->
                        <div class="btn" @click.prevent="sendMsg()">
                            <a href="#">Send Message</a>
                        </div>
                    </div>

                    <!-- Pup up message -->
                    <!-- Se popUp è vero il div appare -->
                    <div class="popup" :class="{'show': popUp}">
                        <span>Your message has been sent!</span>
                    </div>

                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MapAndForm',
    data() {
        return {
            // V-models per input
            name: '',
            email: '',
            subject: '',
            msg: '',
            popUp: false
        }
    },
    methods: {
        // Al click dell'utente se le value delle input sono vuote popUp rimane false, altrimenti popUp diventa vero
        // e dopo 2 secondi popUp ritorno falso
        sendMsg(){
            if (this.name === '' || this.email === '' || this.subject === '' || this.msg === '') {
                this.popUp = false
            } else {
                this.popUp = true
                setTimeout(() => {
                    this.popUp = false
                }, 2000)
                this.name = ''
                this.email = ''
                this.subject = ''
                this.msg = ''
            }
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
@import '../style/btn.scss';

    .section-header {
        text-align: center;
        margin-bottom: 60px;
        h2 {
            margin: 20px 0;
            
        }
        span {
            color: $sub_text;
            font-weight: 500;
        }
    }
    .content {
        display: flex;
        justify-content: space-between;
        position: relative;
        .col {
        width: 55%;
            iframe {
                width: 100%;
                height: 450px;
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
                    font-weight: 500;
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

        .popup {
            display: none;
            width: 400px;
            height: 150px;
            background-color: white;
            border: none;
            box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px, rgba(0, 0, 0, 0.041) 0px 0px 0px 1px;
            text-align: center;
            line-height: 150px;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 10;
            span {
                font-size: 20px;
                font-weight: 500;
            }
        }

        .show {
            display: block;
        }

        .small {
            width: 45%;
            margin-left: 20px;
        }
    }

</style>