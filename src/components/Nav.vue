<template>
    <div>
        <header>
        <div class="logo">
            <a href="index.html" id="name">A | B</a>
        </div>
        <div class="header-menu">
            <a id='scroll-down' class="page-scroll" href="index.html#services-section">Scroll &rarr;</a>
        </div>
        <div class="menu-btn">
            <i class="fas fa-bars"></i>
        </div>
    </header>
    <div class="mobile-menu">
        <a href="index.html">Home</a>
        <a href="index.html#portfolio-section">Portfolio</a>
    </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    header {
        display: flex;
        padding: 20px;
        justify-content: space-between;
        align-items: center;
        position: sticky;
        top: 0;
        align-self: flex-start;
        z-index: 100;
        .logo {
            font-size: 1.5rem;
            font-weight: 350;
            text-transform: uppercase;
            display: flex;
            a#name {
                padding: 15px 20px;
                text-decoration: none;
                color: #222;
                :hover{
                    color:#87cdff;
                }
                :visited{
                    color:#222;
                }
            }
        }
        .header-menu{
            text-transform: uppercase;
            text-decoration: none;
            display: flex;
            justify-content: center;
            align-items: center;
            a.page-scroll{
                font-size: 0.8rem;
                text-decoration: none;
                color: black;
                /* padding: 0 10px; */
                transition: all 0.2s ease-in-out;
                /* Safari */
                -webkit-transform: rotate(90deg);

                /* Firefox */
                -moz-transform: rotate(90deg);

                /* IE */
                -ms-transform: rotate(90deg);

                /* Opera */
                -o-transform: rotate(90deg);

                /* Internet Explorer */
                filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
            }
            a.portfolio-menu{
                font-size: 0.8rem;
                text-decoration: none;
                color: black;
            }
            a:hover{
                color: #87cdff;
            }
        }
    }
</style>