<template>
    <div>
            <section id="portfolio-section">
        <div class="container">
            <div class="title">
                <div class="square"></div>
                <h1>Portfolio</h1>
            </div>
            <div class="portfolio-container">
                <a href="#" class="box image1">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">In progress</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/responsive-projects.html" class="box image2">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">Responsive design</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/api-projects.html" class="box image3">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">RESTful API projects</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/vidly-app-project.html" class="box image4">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">React.js</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/THREEJS-projects.html" class="box image5">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">Three.js</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/sketch-designs.html" class="box image6">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">Sketch Designs</div>
                            </div>
                        </div>
                    </div>
                </a>
                <a href="Portfolio/kid-react-project.html" class="box image7">
                    <div class="image">
                        <div class="hover-bg">
                            <div class="title">
                                <div class="text">Rebuilt on React</div>
                            </div>
                        </div>
                    </div>
                </a>
            </div>
            </div>
    </section>
    </div>
</template>

<script>

    export default {
        components: {
        },
    }
</script>

<style lang="scss" scoped>
    #portfolio-section {
  padding: 80px 120px;

  .title {
    position: relative;
    width: 200px;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;

    .square {
      background: #ffeded;
      width: 150px;
      height: 150px;
      position: absolute;
      top: 23px;
    }

    h1 {
      position: relative;
      font-size: 2.5rem;
      text-transform: uppercase;
      font-weight: 100;
      color: #16171b;
      z-index: 1;
      letter-spacing: 4px;
    }
  }

  .portfolio-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 150px 150px 150px 150px 150px;
    grid-gap: 10px;

    .box {
      background: #f0f0f0;
      display: block;
      transition: all 0.4s ease-in-out;
      cursor: pointer;
      width: 100%;
      color: white;
      text-decoration: none;
      text-transform: uppercase;
      overflow: hidden;
      border-radius: 10px;

      &:hover {
        background: rgba(255, 255, 255, 1);
        -webkit-box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
        -moz-box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
        box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
        cursor: pointer;
      }

      .image .hover-bg {
        padding: 10px 20px;
        background: rgba(255, 255, 255, 0);
        transition: all 0.4s ease-in-out;
        height: 100%;
        width: 100%;
      }

      &:hover .image .hover-bg {
        padding: 10px 20px;
        background: rgba(255, 53, 53, 0.8);

        /* background: rgba(135, 205, 255, 0.8); */
      }

      .image .hover-bg .title {
        height: 100%;
        width: 100%;

        .text {
          background: black;
          border-radius: 5px;
          padding: 10px 20px;
          transform: translate3d(0, 400px, 0);
          transition: all 0.5s ease-in-out;
          opacity: 0;
        }
      }

      &:hover .image .hover-bg .title .text {
        background: black;
        border-radius: 5px;
        padding: 10px 20px;
        transform: translate3d(0, 0px, 0);
        opacity: 1;
      }

      &.image1 {
        grid-column: 1 / 3;
        grid-row: 1 / 2;

        .image {
          background: url("https://cdn.dribbble.com/users/28738/screenshots/4287721/main.jpg");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image2 {
        grid-column: 3 / 4;
        grid-row: 1 / 4;

        .image {
        //   background: url("../portfolio/images/Screen Shot 2018-11-01 at 12.13.34-fullpage");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image3 {
        grid-column: 1 / 2;
        grid-row: 2 / 4;

        .image {
          /* background: url("https://cdn.dribbble.com/users/1094383/screenshots/4107773/800x600_5.gif"); */
          /* background: url("../portfolio/images/poke-api.png"); */
        // new  background: url("../portfolio/images/poke-sc.png");
          height: 100%;
          width: 100%;

          /* object-fit: cover; */
          background-size: contain;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image4 {
        grid-column: 2 / 3;
        grid-row: 2 / 3;

        .image {
        //   background: url("../portfolio/images/Optimized-Screen(1)");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image5 {
        grid-column: 1 / 2;
        grid-row: 4 / 6;

        .image {
          /* old background: url("../portfolio/images/orbit-geo.gif"); */
        // new  background: url("../portfolio/images/geometry-space");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image6 {
        grid-column: 2 / 3;
        grid-row: 3 / 6;

        .image {
        //   background: url("https://cdn.dribbble.com/users/952958/screenshots/3990931/decor..png");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }

      &.image7 {
        grid-column: 3 / 4;
        grid-row: 4 / 6;

        .image {
        //   background: url("../portfolio/images/Optimized-Screen");
          height: 100%;
          width: 100%;
          background-size: cover;
          background-position: center center;
          background-repeat: no-repeat;
        }
      }
    }
  }
}

/* Box locations */

/* Box1 */

/* Box2 */

/* Box3 */

/* Box4 */

/* Box5 */

/* Box6 */

/* Box7 */

/*Tablets */
@media only screen and (max-width: 960px) {
  #portfolio-section .portfolio-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 150px 150px 150px 150px 150px 150px 150px;
    grid-gap: 10px;

    .box {
      &.image1 {
        grid-column: 1 / 2;
        grid-row: 1 / 3;
      }

      &.image2 {
        grid-column: 2 / 3;
        grid-row: 1 / 3;
      }

      &.image3 {
        grid-column: 1 / 2;
        grid-row: 3 / 5;
      }

      &.image4 {
        grid-column: 2 / 3;
        grid-row: 3 / 5;
      }

      &.image5 {
        grid-column: 1 / 2;
        grid-row: 5 / 7;
      }

      &.image6 {
        grid-column: 2 / 3;
        grid-row: 5 / 7;
      }

      &.image7 {
        grid-column: 1 / 4;
        grid-row: 7 / 9;
      }
    }
  }
}
@media only screen and (max-width: 767px) {
  #portfolio-section .portfolio-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 150px 150px 150px 150px 150px 150px;
    grid-gap: 10px;

    .box {
      &.image1 {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
      }

      &.image2 {
        grid-column: 1 / 4;
        grid-row: 2 / 3;
      }

      &.image3 {
        grid-column: 1 / 4;
        grid-row: 3 / 4;
      }

      &.image4 {
        grid-column: 1 / 4;
        grid-row: 4 / 5;
      }

      &.image5 {
        grid-column: 1 / 4;
        grid-row: 5 / 6;
      }

      &.image6 {
        grid-column: 1 / 4;
        grid-row: 6 / 7;
      }

      &.image7 {
        grid-column: 1 / 4;
        grid-row: 7 / 8;
      }
    }
  }
}
/*Phone*/
@media only screen and (max-width: 450px) {
  #portfolio-section {
    padding: 40px 45px;

    .title {
      .square {
        width: 95px;
        height: 95px;
        top: 54px;
        left: 45px;
      }

      h1 {
        right: 4px;
        font-size: 1rem;
        font-weight: 100;
      }
    }
  }
}
</style>