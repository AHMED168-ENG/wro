<template>
    <nav>
        <div class="container">
            <div class="d-flex nav-wrapper">
                <div class="left">
                    <div class="image">
                        <a href="">
                            <img src="../../assets/nav1.png" alt="">
                        </a>
                    </div>
                    <div class="image">
                        <a href="">
                            <img src="../../assets/nav2.png" alt="">
                        </a>
                    </div>
                </div>
                <div class="right">
                    <div class="image ">
                        <a href="">
                            <img src="../../assets/nav3.png" alt="">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name:"NavbarComponent"
}
</script>

<style lang="scss" scoped>
@import "../../scss/variables.scss";

nav {
    z-index: 100;
    background: $main-color;
    padding:17px 0;
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100px;
    * {
        height:100%
    }
    .nav-wrapper {
        flex-wrap: wrap;
        justify-content: space-between;
        .left {
            width:22%;
            display: flex;
            .image {
                flex-grow: 1;
            }
            .image:nth-of-type(1) {
                margin-left:30px
            }
        }
        .right {
            width:40%;
            display: flex;
            justify-content: end;
        }
        .image {
            img {
                width:100%;
                object-fit: contain;
            }
        }

    }

    
}
  
@media (max-width: 1500px) {
        nav .nav-wrapper .left {
        width:30% 
    }
}
@media (max-width: 1300px) {


}

@media (max-width: 1000px) {
    nav .nav-wrapper .left {
        width:55% 
    }
}

@media (max-width: 700px) {

}
@media (max-width: 400px) {
}
</style>