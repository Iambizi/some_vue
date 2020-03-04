<template>
    <div>
        <section id="top">
            <div class="container">
                <div class="info">
                    <h1>Amir Bizimana<span class="punctuation">,</span> Front-end Dev.
                    </h1>
                    <p id="about">About me</p>
                    <p id="about-text">Welcome to my portfolio site.
                        <br>I'm a self taught Front-end developer, currently based in Canada.
                        <br>Stay tuned for upcoming projects showcasing new skills I pick up.</p>
                    <a id="latest" href="#portfolio-section">Latest Work</a>
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
    #top {
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            padding: 80px 10px;
            align-items: center;
        }
        .info {
            padding: 15px;
            height: 60vh;

            h1 {
            font-size: 5.5rem;
            text-transform: capitalize;
            font-weight: 700;
            color: #16171b;
            margin-bottom: 2rem;
            word-break: keep-all;
            }

            .punctuation {
            font-family: "karla", sans-serif;

            /* font-size: 4rem; */
            }

            p {
            /* position: relative; */
            color: #919191;
            margin-bottom: 2rem;
            z-index: 1;
            cursor: pointer;
            }

            #about:hover {
            color: #87cdff;
            }
        }
}

#about {
  font-size: 0.7rem;
}

#top {
  .info {
    p#about-text {
      display: none;
    }

    #latest {
      color: #000;
      font-weight: 600;
      text-transform: uppercase;
      text-decoration: none;
      padding-bottom: 5px;
      border-bottom: 2px solid #87cdff;
      letter-spacing: 2px;
    }
  }

  .img .background-img {
    // background: url("../../img/newcssimg.png");
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    max-width: 500px;
    height: 800px;
    margin: 0 auto;
  }
}

@media only screen and (max-width: 1280px) {
  #top .container {
    padding: 19px 25px 80px 70px;
  }
}

/*Tablets */
@media only screen and (max-width: 960px) {
  #top {
    .container {
      padding: 50px 25px 80px 55px;
    }

    .info .blue-square {
      display: none;
    }

    .img .background-img {
      height: 100vh;
    }

    .info h1 {
      font-size: 5.5rem;
    }
  }
}

/*Phone*/
@media only screen and (max-width: 767px) {
  #top .info {
    h1 {
      font-size: 3.2rem;
    }

    p#about-text {
      font-size: 0.7rem;
    }
  }
}

@media only screen and (max-width: 400px) {
  #top {
    .container {
      padding: 30px 25px;
    }

    .info {
      h1 {
        font-size: 3.2rem;
      }

      #latest {
        letter-spacing: 0.8px;
        font-size: 0.8rem;
      }

      p#about-text {
        font-size: 0.5rem;
      }
    }
  }
}
</style>