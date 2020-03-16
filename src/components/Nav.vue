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
}
header .logo {
  font-size: 1.5rem;
  font-weight: 350;
  text-transform: uppercase;
  display: flex;
}
header div.logo a#name {
  padding: 15px 20px;
  text-decoration: none;
  color: #222;
}
header div.logo a#name:hover {
  color: #87cdff;
}

header .logo #name:visited {
  color: #222;
}
header .header-menu {
  text-transform: uppercase;
  text-decoration: none;
  display: flex;
  justify-content: center;
  align-items: center;
}
header .header-menu a.page-scroll {
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
header .header-menu a.portfolio-menu {
  font-size: 0.8rem;
  text-decoration: none;
  color: black;
}
header .header-menu a:hover {
  color: #87cdff;
}
header .menu-btn {
  font-weight: 700;
  color: #87cdff;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 15px;
  font-size: 1.6rem;
  display: none;
  cursor: pointer;
}
.mobile-menu {
  display: none;
  background: #fff;
  flex-direction: column;
  padding: 40px 0;
  position: absolute;
  top: 0;
  height: 100vh;
  width: 50%;
  z-index: 10;
  transform: translate3d(-100%, 0, 0);
  transition: all 0.4s ease-in-out;
}
.mobile-menu.active {
  transform: translate3d(0, 0, 0);
}
.mobile-menu a {
  padding: 15px;
  text-decoration: none;
  color: black;
}

.mobile-menu a:hover {
  text-decoration: none;
  color: #87cdff;
}
@media only screen and (max-width: 960px) {
  .container {
    width: 100%;
  }
}
@media only screen and (max-width: 767px) {
  header .header-menu a.page-scroll:visited {
    color: #000;
  }
}
</style>