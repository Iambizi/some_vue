<template>
    <div>
        <section id="services-section">
            <div class="container">
                <div class="title">
                    <div class="circle"></div>
                    <h1>Skills</h1>
                </div>
                <div class="services-container">
                    <div class="box blue">
                        <i class="fas fa-trophy"></i>
                        <h5>Core</h5>
                        <p>
                            <ul>HTML</ul>
                            <ul>CSS / SASS</ul>
                            <ul>JavaScript</ul>
                            <ul>Git</ul>
                            <ul>Mobile and responsive design</ul>
                            <ul>Sketch</ul>
                        </p>
                    </div>
                    <div class="box red">
                        <i class="fas fa-fighter-jet"></i>
                        <h5>Libraries / Frameworks</h5>
                        <p>
                            <ul>Boostrap</ul>
                            <ul>jQuery</ul>
                            <ul>Gulp</ul>
                            <ul>Webpack-Encore</ul>
                        </p>
                    </div>
                    <div class="box yellow">
                        <i class="fas fa-money-bill-wave-alt"></i>
                        <h5>Currently learning</h5>
                        <ul>Redux</ul>
                        <ul>Webpack</ul>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
#services-section {
  padding: 80px 120px;
}

#services-section .title {
  position: relative;
  width: 200px;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
}

#services-section .title .circle {
  background: #eef9ff;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  position: absolute;
  top: 23px;
}
#services-section .title h1 {
  position: relative;
  font-size: 2.5rem;
  text-transform: uppercase;
  color: #16171b;
  font-weight: 100;
  letter-spacing: 4px;
}

#services-section .services-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 40px;
}

#services-section .services-container .box {
  background: rgba(255, 255, 255, 0);
  transition: all 0.4s ease-in-out;
  padding: 40px;
  cursor: pointer;
}

#services-section .services-container .box:hover {
  background: rgba(255, 255, 255, 1);
  -webkit-box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
  -moz-box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
  box-shadow: 10px 40px 74px 24px rgba(0, 0, 0, 0.08);
}

#services-section .services-container .box .fas {
  font-size: 2rem;
  margin-bottom: 2rem;
}

#services-section .services-container .box h5 {
  font-size: 0.9rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 2px;
  margin-bottom: 2rem;
}

#services-section .services-container .box ul,
p {
  font-size: 0.8rem;
  line-height: 1.5;
  color: #b3b3b3;
}

#services-section .services-container .box.blue {
  border-bottom: 2px solid #52b8ff;
}

#services-section .services-container .box.red {
  border-bottom: 2px solid #ff5253;
}

#services-section .services-container .box.yellow {
  border-bottom: 2px solid #ffc853;
}

/*Tablets */
@media only screen and (max-width: 960px) {
  #services-section .services-container {
    grid-template-columns: 100%;
  }
  #services-section .services-container .box:hover {
    background: rgba(255, 255, 255, 1);
    -webkit-box-shadow: 0px 40px 74px 24px rgba(0, 0, 0, 0.08);
    -moz-box-shadow: 0px 40px 74px 24px rgba(0, 0, 0, 0.08);
    box-shadow: 0px 40px 74px 24px rgba(0, 0, 0, 0.08);
  }
}

@media only screen and (max-width: 767px) {
}
/*Phone*/
@media only screen and (max-width: 450px) {
  #services-section .title .circle {
    width: 100px;
    height: 100px;
    top: 53px;
    left: 45px;
  }
  #services-section {
    padding: 35px 45px;
  }
  #services-section .title h1 {
    right: 4px;
    font-size: 1rem;
    font-weight: 100;
  }
  #services-section .services-container .box .fas {
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }

  #services-section .services-container .box h5 {
    font-size: 0.7rem;
  }

  #services-section .services-container .box ul,
  p {
    font-size: 0.6rem;
  }
}
</style>