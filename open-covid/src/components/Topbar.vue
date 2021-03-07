<template>
<div>
  <div id="topbar" class="d-flex align-items-center fixed-top">
    <div class="container d-flex align-items-center justify-content-center justify-content-md-between">
      <div class="align-items-center d-none d-md-flex">
        <i class="bi bi-envelope-fill"></i> Contactanos: informes@insightcovid.com
      </div>
      <div class="d-flex align-items-center">
        <i class="bi bi-phone"></i> Llamanos: +51 965588142
      </div>
    </div>
  </div>
</div>
  
</template>

<script>
export default {
  name: 'Topbar',
  props: {
    msg: String
  }
}
</script>

<style scoped>

/*--Top Bar--*/

#topbar {
  background: #AD1522;
  color: #fff;
  height: 40px;
  font-size: 16px;
  font-weight: 600;
  z-index: 996;
  transition: all 0.5s;
}

#topbar.topbar-scrolled {
  top: -40px;
}

#topbar i {
  padding-right: 6px;
  line-height: 0;
}

</style>
