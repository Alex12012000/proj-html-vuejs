<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/logo-2.png" alt="logo">
        </div>
        <div class="header-content">
            <div class="menu">
                <ul>
                    <li v-for="el, index in headerMenu" :key="index">{{el}}</li>
                </ul>
            </div>
            <div class="icons">
                <i class="fa-solid fa-magnifying-glass"></i>
                <i class="fa-solid fa-cart-shopping"></i>
                <div class="blue-circle">
                    0
                </div>
            </div>
            <div class="btn">
                <a href="#">Get Started</a>
            </div>
        </div>

    </header>
</template>

<script>
export default {
    name: 'PageHeader',
    props: {
        headerMenu: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../style/btn.scss';
@import '../style/vars.scss';

header {
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 10px;

    .logo {
        width: 40px;
    }

    .header-content {
        display: flex;
        align-items: center;
        height: 100%;

        .menu {
            ul {
                display: flex;
                line-height: 70px;
            }
            li {
                list-style-type: none;
                margin: 0 10px;
            }
            li:first-child {
                color: $main_color;
                box-shadow: inset 0px -11px 1px -9px $main_color; 
            }
        }

        .icons {
            position: relative;
            margin: 0 20px;
            i {
                margin: 0 10px;
                font-size: 13px;
                position: relative;
                z-index: 2;
            }
            .blue-circle {
                width: 15px;
                height: 15px;
                line-height: 15px;
                text-align: center;
                border-radius: 50%;
                font-size: 10px;
                background-color: $main_color;
                color: white;
                position: absolute;
                top: -5px;
                right: 0;
                z-index: 0;
            }
        }

        a {
            text-decoration: none;
            color: inherit;
        }
    }
}


</style>