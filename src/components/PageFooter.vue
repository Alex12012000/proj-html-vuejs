<template >
    <footer>
        <div class="container">
            <div class="content">
                <!-- Brand Info -->
                <div class="page-info">
                    <!-- Logo -->
                    <img src="../assets/img/35.png" alt="logo">
                    
                    <p>It is a long established fact that a reader will be distracted by the readable content.</p>

                    <span>Copyright @ 2018 <a href="#">Sofbox</a></span>
                </div>

                <!-- Nav Links -->
                <div class="footerlinks">

                    <div class="list">
                        <h4>Menu</h4>
                        <ul>
                            <!-- Menu Li creati con v-for e props -->
                            <li v-for="el, index in menuLinks" :key="index">
                                <a href="#">{{el}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="list">
                        <h4>About Us</h4>
                        <ul>
                            <li v-for="el, index in aboutLinks" :key="index"> 
                                <a href="#">{{el}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="list">
                        <h4>Quick Link</h4>
                        <ul>
                            <li v-for="el, index in aboutLinks" :key="index">
                                <a href="#">{{el}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="arrow">
            <a href="#jumbo"><i class="fa-solid fa-chevron-up"></i></a>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'PageFooter',
    props: {
        menuLinks: Array,
        aboutLinks: Array
    }
}
</script>
<style lang="scss" scoped>
@import '../style/btn.scss';
@import '../style/vars.scss';

    footer {
        border-top: 1px solid lightgrey;
        padding: 50px 0;
        position: relative;
        .content {
            display: flex; 
            align-items: center;
            .page-info {
            width: 30%;
                img {
                    width: 130px;
                }
                p {
                    font-size: 13px;
                    margin-top: 15px;
                }
                span {
                    display: block;
                    margin: 30px 0;
                    color: $sub_text;
                    font-size: 13px;
                    font-weight: 500;
                    a {
                        color: $main_color;
                    }
                }
            }

            .footerlinks {
                width: 100%;
                display: flex;
                justify-content: space-around;
                .list {
                    h4 {
                        margin-bottom: 25px;
                    }
                    li {
                        display: flex;
                        flex-direction: column;
                        margin: 10px 0;
                        a {
                            font-size: 14px;
                            color: $sub_text;
                        }
                    }
                }
            }
        }

        .arrow {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: lightgray;
            color: white;
            text-align: center;
            line-height: 50px;
            font-size: 18px;
            position: absolute;
            bottom: 50px;
            right: 50px;
        }
    }
</style>