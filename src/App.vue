<script setup>
  import "bootstrap/dist/css/bootstrap.css"
  import "font-awesome/css/font-awesome.css"

  const prefixes = ["Air", "Jet", "Flight"];
  const sufixes = ["Hub", "Station", "Mart"];
  const domains = ["AirHub", "AirStation", "AirMart", "JetHub", "JetStation", "JetMart", "FlighHub", "FlighStation", "FlightMart"];
</script>

<template>
  <div>
    <div class="text-center">
      <h1>NameGator</h1>
      <br>
      <h6 class="text-secondary">Gerador de nomes utilizando Vue.js GraphQL e Node</h6>
    </div>
    <div id="main">
      <div class="container">
        <div class="row">
          <div class="col-md">
            <h5>Prefixos <span class="badge badge-primary">{{ prefixes.length }}</span></h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item" v-for="prefix in prefixes" v-bind:key="prefix">
                    {{ prefix }}
                  </li>
                </ul>
                <br>
                <input type="text" class="form-control" placeholder="Digite o prefixo ">

              </div>
            </div>
          </div>
          <div class="col-md">
            <h5>Prefixos <span class="badge badge-info">{{ sufixes.length }}</span></h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item" v-for="sufix in sufixes" v-bid:key="sufix">
                    {{ sufix }}
                  </li>
                </ul>
                <br>
                <input type="text" class="form-control" placeholder="Digite o sufixo">
              </div>
            </div> 
          </div>
        </div>
        <br>
        <div class="col-md">
          <h5>Prefixos <span class="badge badge-primary">{{ domains.length }}</span></h5>
          <div class="card">
            <div class="card-body">
              <ul class="list-group">
                <li class="list-group-item" v-for="domain in domains" v-bid:key="domain">
                  {{ domain }}
                </li>
              </ul>
              <br>
              <input type="text" class="form-control" placeholder="Digite o sufixo">
            </div>
          </div> 
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
#slogan {
  margin-top: 30px;
  margin-bottom: 30px;
}

#main {
  background-color: #F1F1F1;
  padding-top: 30px;
  padding-bottom: 30px;
}
</style>
