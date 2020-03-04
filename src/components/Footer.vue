<template>
    <div>
        <footer>
            <div class="social-container">
                <!-- <a href="http://www.instagram.com/iambizi">
                    <i class="fab fa-instagram"></i>
                </a> -->
                <a href="http://www.linkedin.com/in/amir-bizimana-349169122/">
                    <i class="fab fa-linkedin-in"></i>
                    <font-awesome-icon :icon="linkedin" />
                </a>
                <a href="http://www.github.com/iambizi">
                    <i class="fab fa-github"></i>
                </a>
                <a href="http://www.twitter.com/Amirbizi">
                    <i class="fab fa-twitter"></i>
                </a>
                <a href="https://medium.com/@Iambizi">
                    <i class="fab fa-medium"></i>
                </a>	
            </div>
            <h5>&copy; 2020 Amir Bizimana</h5>
        </footer>
    </div>
</template>
<script>

    export default {

    }
</script>

<style lang="scss" scoped>
    footer{
        background: #f9fafc;
        padding: 100px 15px;
        .scocial-container{
            display: grid;
            grid-template-columns: 1fr 1fr 1fr 1fr;
            justify-items: center;
            align-items: center;
            max-width: 400px;
            margin: 0 auto;
            a {
                font-size: 3rem;
                color: #aeaf91;
                text-decoration: none;
                transition: all 0.3s ease-in-out;
                display: inline-block;
                padding: 10px;
                :hover{
                    color: rgba(255, 53, 53,1);
                }
            }
        }
        h5 {
            font-size: 0.8rem;
            color: black;
            text-transform: capitalize;
            text-align: center;
            margin: 20px 0;
        }
        h6 {
            font-size: 0.8rem;
            color: black;
            text-transform: capitalize;
            text-align: center;
        }
        @media only screen and (max-width: 767px) {
            footer .social-container a {
                font-size: 2.5rem;
            }
        }
        @media only screen and (max-width: 450px) {
            footer .social-container a {
                font-size: 2rem;
            }
        }
    }
</style>