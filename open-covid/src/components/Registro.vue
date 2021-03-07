<template>

<div class="row fondo-Registro fixed-top">
    <div class="col-lg-4">

    </div>

    <div class="col-lg-4 mt-5 text-center">
        <br>
        <br>
        <br>
        <h1><strong>Completa el Formulario de Registro </strong> </h1> 
<div class="card " >
  <div class="card-body">  
      <form >

   <div class="input-group mb-3"> 
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Nombres <span class="text-danger">*</span></label>
                <input type="text" class="form-control" placeholder="Ingresa tus nombres">
         </div>
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Apellido Paterno <span class="text-danger">*</span></label>
            <input type="text" class="form-control" placeholder="Ingresa tus apellido paterno">
        </div>
    </div>

    <div class="input-group mb-3"> 
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Apellido Materno <span class="text-danger">*</span></label>
                <input type="text" class="form-control" placeholder="Ingresa tu apellido Materno">
         </div>
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Fecha de Nacimiento <span class="text-danger">*</span></label>
            <input type="date" class="form-control" placeholder="">
        </div>
    </div>

    <div class="input-group mb-3"> 
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Distrito de Residencia <span class="text-danger">*</span></label>
                <input type="text" class="form-control" placeholder="Ingresa tu distrito">
         </div>
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Distrito Recurrente o Trabaja <span class="text-danger">*</span></label>
            <input type="text" class="form-control" placeholder=" Ingresa tu distrito recurrente ">
        </div>
    </div>

  <div class="input-group mb-3"> 
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Correo <span class="text-danger">*</span></label>
                <input type="email" class="form-control" placeholder="Ingresa tu correo">
         </div>
        <div class="form-group col-md-6">
            <label class="font-weight-bold">Contraseña <span class="text-danger">*</span></label>
            <input type="password" class="form-control" placeholder="Ingrea tu contraseña">
        </div>
    </div>

  <button type="submit" class="btn btn-success">Enviar</button>
</form>
  </div>
</div>
    </div>

    <div class="col-lg-4">
      
    </div>
</div>
</template>

<script>
export default {

}
</script>

<style>

/*--Registro--*/

.fondo-Registro {
  color:#AD1522;
  background-image: url(../assets/img/slide/fondo-2.jpg);
  background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    height: 100%;
    padding-top: -500px;

}

</style>