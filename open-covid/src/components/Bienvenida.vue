<template>
<div>

  <div id="fondo" class="d-flex align-items-center fixed-top">
      <header id="header" class="fixed-top">
    <div class="container d-flex align-items-center">

      <a href="" class="logo me-auto"><img src="" alt=""></a>

      <nav id="navbar" class="navbar order-last order-lg-0">
        <ul>
          <li><a class="nav-link scrollto">Inicio</a></li>
        </ul>
        <i class="bi bi-list mobile-nav-toggle"></i>
      </nav>

      <a href="#appointment" style="text-decoration:none" class="appointment-btn scrollto"><span class="d-none d-md-inline"></span>Cerrar Sesión</a>

    </div>
  </header>
    <div class="container">
        <div class="row section">
            <div class="col-lg-6">
                <div class="mt-3">
                      <img src="../assets/images/Video.png" class="image" alt=""> <button type="button" class="btn btn-warning ">Warning</button>
                </div>

                <div class="mt-4">
                      <img src="../assets/images/Estadisticas.png" class="image" alt=""> <button type="button" class="btn btn-warning mt-3">Warning</button>
                </div>
                
                <div class="mt-4">
                     <img src="../assets/images/Balon-de-Oxigeno.png" class="image" alt="">   <button type="button" class="btn btn-warning mt-3">Warning</button>
                </div>
                  
                <div class="mt-4">
                    <img src="../assets/images/Cama-UCI.png" class="image" alt="">   <button type="button" class="btn btn-warning mt-3">Warning</button>
                </div>

                  
                
                
            </div>

            <div class="col-lg-6">
                Hola
            </div>
        </div>
    </div>
  </div>
</div>
  
    

    
</template>

<script>
export default {

}
</script>

<style>

/*--Top Bar--*/

#fondo {
    color: #fff;
    background-image: url(../assets/images/Fondo.png);
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    height: 100vh;
}

.section {
    margin-right: 400px;
}

.image{
    width: 120px;
    height: 120px;
}

/*--Header--*/

#header {

  transition: all 0.5s;
  z-index: 997;
  padding: 20px 0;
  top: 0px;
  box-shadow: 0px 2px 15px rgba(0, 0, 0, 0.1);
}

@media (max-width: 992px) {
  #header {
    padding: 15px 0;
  }
}

  #header.header-scrolled {
  top: 0;
}

  #header .logo {
  font-size: 28px;
  margin: 0;
  padding: 0;
  line-height: 1;
  font-weight: 600;
  letter-spacing: 0.5px;
  text-transform: uppercase;
}

#header .logo a {
  color: #555555;
}

#header .logo img {
  max-height: 40px;
}

.appointment-btn {
  margin-left: 25px;
  background: #AD1522;
  color: #fff;
  border-radius: 4px;
  padding: 8px 25px;
  white-space: nowrap;
  transition: 0.3s;
  font-size: 14px;
  display: inline-block;
}


@media (max-width: 768px) {
  .appointment-btn {
    margin: 0 15px 0 0;
    padding: 6px 15px;
  }
}

.navbar {
  padding: 0;
}

.navbar ul {
  margin: 0;
  padding: 0;
  display: flex;
  list-style: none;
  align-items: center;
}

.navbar li {
  position: relative;
}

.navbar a {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 0 10px 30px;
  font-family: "Roboto", sans-serif;
  font-size: 13px;
  color: #626262;
  white-space: nowrap;
  transition: 0.3s;
  text-transform: uppercase;
  font-weight: 500;
}

.navbar a i {
  font-size: 12px;
  line-height: 0;
  margin-left: 5px;
}

.navbar a:hover, .navbar .active, .navbar li:hover > a {
  color: #AD1522;
}

.navbar .dropdown ul {
  display: block;
  position: absolute;
  left: 14px;
  top: calc(100% + 30px);
  margin: 0;
  padding: 10px 0;
  z-index: 99;
  opacity: 0;
  visibility: hidden;
  background: #fff;
  box-shadow: 0px 0px 30px rgba(127, 137, 161, 0.25);
  transition: 0.3s;
  border-radius: 4px;
}

.navbar .dropdown ul li {
  min-width: 200px;
}

.navbar .dropdown ul a {
  padding: 10px 20px;
  text-transform: none;
}

.navbar .dropdown ul a i {
  font-size: 12px;
}

.navbar .dropdown:hover > ul {
  opacity: 1;
  top: 100%;
  visibility: visible;
}

.navbar .dropdown .dropdown ul {
  top: 0;
  left: calc(100% - 30px);
  visibility: hidden;
}

.navbar .dropdown .dropdown:hover > ul {
  opacity: 1;
  top: 0;
  left: 100%;
  visibility: visible;
}

@media (max-width: 1366px) {
  .navbar .dropdown .dropdown ul {
    left: -90%;
  }
  .navbar .dropdown .dropdown:hover > ul {
    left: -100%;
  }
}


.mobile-nav-toggle {
  color: #555555;
  font-size: 28px;
  cursor: pointer;
  display: none;
  line-height: 0;
  transition: 0.5s;
}

.mobile-nav-toggle.bi-x {
  color: #fff;
}

@media (max-width: 991px) {
  .mobile-nav-toggle {
    display: block;
  }
  .navbar ul {
    display: none;
  }
}

.navbar-mobile {
  position: fixed;
  overflow: hidden;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background: rgba(60, 60, 60, 0.9);
  transition: 0.3s;
  z-index: 999;
}

.navbar-mobile .mobile-nav-toggle {
  position: absolute;
  top: 15px;
  right: 15px;
}

.navbar-mobile ul {
  display: block;
  position: absolute;
  top: 55px;
  right: 15px;
  bottom: 15px;
  left: 15px;
  padding: 10px 0;
  border-radius: 8px;
  background-color: #fff;
  overflow-y: auto;
  transition: 0.3s;
}

.navbar-mobile a {
  padding: 10px 20px;
  font-size: 15px;
  color: #555555;
}

.navbar-mobile a:hover, .navbar-mobile .active, .navbar-mobile li:hover > a {
  color: #AD1522;
}

.navbar-mobile .dropdown ul {
  position: static;
  display: none;
  margin: 10px 20px;
  padding: 10px 0;
  z-index: 99;
  opacity: 1;
  visibility: visible;
  background: #fff;
  box-shadow: 0px 0px 30px rgba(127, 137, 161, 0.25);
}

</style>