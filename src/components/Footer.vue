<template>
    <section>
        <div class="container">

            <div class="row">
                
                <div class="col-left">
                    <span class="title">
                        Address
                    </span>

                    <span class="info">

                        382 NE 191st St # 87394 Miami, FL 33179-3899 <br>
                        +1(305) 547-9909 (9am - 5pm EST, Monday - Friday) <br>
                        support@maxcoach.com
                    </span>

                    <ul>

                        <li class="icon-social">
                            <a href="#">
                                <i class="fab fa-facebook-square"></i>
                            </a>
                        </li>

                        <li class="icon-social">
                            <a href="#">
                                <i class="fab fa-twitter"></i>
                            </a>
                        </li>

                        <li class="icon-social">
                            <a href="#">
                                <i class="fab fa-instagram"></i>
                            </a>
                        </li>

                        <li class="icon-social">
                            <a href="#">
                                <i class="fab fa-linkedin"></i>
                            </a>
                        </li>
                    </ul>

                </div>

                <div class="col-right">

                    <div class="row">

                        <!-- first column link -->
                        <div class="first-nav">

                            <span class="title">
                                Explore
                            </span>

                            <div class="container-link">

                                <ul>

                                    <li>
                                        <a href="#">Start here</a>
                                    </li>

                                    <li>
                                        <a href="#">Blog</a>
                                    </li>

                                    <li>
                                        <a href="#">About us</a>
                                    </li>
                                </ul>

                                <ul>
                                    <li>
                                        <a href="#">Success Story</a>
                                    </li>

                                    <li>
                                        <a href="#">Courses</a>
                                    </li>

                                    <li>
                                        <a href="#">Contact us</a>
                                    </li>
                                </ul>
                            </div>

                        </div>

                        <!-- second column link -->
                        <div class="second-nav">

                            <span class="title">
                                Information
                            </span>

                            <ul>

                                <li>
                                    <a href="#">Membership</a>
                                </li>

                                <li>
                                    <a href="#">Purchase guide</a>
                                </li>

                                <li>
                                    <a href="#">Privacy policy</a>
                                </li>

                                <li>
                                    <a href="#">Terms of service</a>
                                </li>
                            </ul>

                        </div>

                    </div>

                </div>
            </div>

            <div class="final-footer-section">
                <span>
                    <i class="far fa-copyright"></i>
                    2020 Maxcoach. All Rights Reserved
                </span>
            </div>

        </div>
    </section>
</template>

<script>
export default {
name: 'Footer;'
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

.row{
    display: flex;
}

span{
    display: block;
    margin-bottom: 15px;
}

.col-left{
    width: 50%;

    .info{
        line-height: 30px;
    }

    ul{
        display: flex;
        list-style: none;

        .icon-social{
            margin: 0 10px;

            a{
                cursor: pointer;

                i{
                    font-size: 22px;
                    color: white;
                    cursor: pointer;
                }
            }
        }
    }
}


.title{
    font-weight: bold;
    font-size: 18px;
}

.col-right{
    width: 50%;

    .row{

        .first-nav{
            margin-right: 80px;

            .container-link{
                display: flex;

                ul:first-of-type{
                    margin-right: 40px;
                }
            }
        }
    
        .first-nav,
        .second-nav{
    
            ul{
                list-style: none;
                line-height: 30px;
    
                a{
                    text-decoration: none;
                    color: white;
                }
            }
        }
    }
}

.final-footer-section{
    width: 100%;
    text-align: center;
    margin-top: 30px;
}


</style>