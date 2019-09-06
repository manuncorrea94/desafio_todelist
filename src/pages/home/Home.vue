<template>

<div class="">
<!--Menu-->

<div class="menu">
  <ul class="nav justify-content-end container">
  <li class="nav-item">
    <a class="nav-link active" href="#">Home</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Formulario</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Relatorio</a>
  </li>
  </ul>
</div><!--Fim do menu-->

<div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
  <h1 class="display-4">To Do List</h1>
  <p class="lead">Os códigos da tarefa devera ser disponibilizado no GitHub</p>
</div>

<!--Formulario-->
<form>
  <div class="container">
  <div class="form-row">

    <div class="form-group col-md-4">
      <label for="inoutText">Titulo do Produto:</label>
      <input type="email" class="form-control" id="inputEmail4" placeholder="Titulo">
    </div>

    <div class="form-group col-md-8">
      <label for="inoutDescription">Descrição:</label>
      <input type="email" class="form-control" id="inputEmail4" placeholder="Descrição">
    </div>

    <div class="form-group col-md-4">
      <label for="inoutPontuacao">Pontuação Numerica:</label>
        <select class="form-control" id="exampleFormControlSelect1">
          <option>1</option>
          <option>2</option>
          <option>3</option>
          <option>4</option>
          <option>5</option>
          <option>6</option>
          <option>7</option>
          <option>8</option>
          <option>9</option>
          <option>10</option>
          <option>11</option>
          <option>12</option>
          <option>13</option>
      </select>
    </div>

    <div class="form-group col-md-4">
      <label for="inoutDia">Dia:</label>
      <input type="text" class="form-control" id="calendario" >
    </div>

  </div>
  <button type="button" class="btn btn-success">Adicionar</button>
  <button type="button" class="btn btn-primary">Gerar Dias</button>
  </div>
</form><!--fim formulario-->

<div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
  <h6 class="display-4">Gerar Relatorio</h6>
</div>
</div>


</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}

$(function() {
	    $( "#calendario" ).datepicker();
	});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.menu{
  background: #007bff!important;
  height: 70px;
}

.nav-link{
  color: #fff;
  margin-top: 10px;
}

h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
