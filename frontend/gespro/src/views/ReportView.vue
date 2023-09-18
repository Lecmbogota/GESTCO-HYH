<template>
    <nav class="navbar navbar-light bg-light justify-content-start">
      <div class="col-6 d-flex justify-content-start align-items-center px-3">
        <a class="navbar-brand" href="/">
          <img :src="Logo" alt="logo" class="img-fluid" style="height: 30px;" />
        </a>
      </div>
      <div class="col-6 d-flex justify-content-end">
        <a class="nav-link px-4" href="/"> <font-awesome-icon :icon="['fas', 'right-to-bracket']" />SALIR</a>
      </div>
    </nav>
    <div class="tab-content">
      <router-view></router-view>
    </div>
  
  <!-- Nav tabs -->
  <ul class="nav nav-tabs mt-4" id="myTab" role="tablist">
    <li class="nav-item" role="presentation">
      <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home" type="button" role="tab" aria-controls="home" aria-selected="true">Dashboard</button>
    </li>
    <li class="nav-item" role="presentation">
      <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#profile" type="button" role="tab" aria-controls="profile" aria-selected="false">Cargar Nuevo Reporte</button>
    </li>
    <li class="nav-item" role="presentation">
      <button class="nav-link" id="messages-tab" data-bs-toggle="tab" data-bs-target="#messages" type="button" role="tab" aria-controls="messages" aria-selected="false">Departamentos</button>
    </li>
    <li class="nav-item" role="presentation">
      <button class="nav-link" id="messages-tab" data-bs-toggle="tab" data-bs-target="#messages" type="button" role="tab" aria-controls="messages" aria-selected="false">Roles</button>
    </li>
    <li class="nav-item" role="presentation">
      <button class="nav-link" id="messages-tab" data-bs-toggle="tab" data-bs-target="#messages" type="button" role="tab" aria-controls="messages" aria-selected="false">Logs</button>
    </li>
  </ul>
  
  <!-- Tab panes -->
  <div class="tab-content">
    <div class="tab-pane active" id="home" role="tabpanel" aria-labelledby="home-tab"><Roles></Roles></div>
    <div class="tab-pane" id="profile" role="tabpanel" aria-labelledby="profile-tab"> Usuarios </div>
    <div class="tab-pane" id="messages" role="tabpanel" aria-labelledby="messages-tab"> Departamentos </div>
    <div class="tab-pane" id="messages" role="tabpanel" aria-labelledby="messages-tab"> Roles </div>
    <div class="tab-pane" id="messages" role="tabpanel" aria-labelledby="messages-tab"> Logs </div>
  </div>
  
  </template>
  
  <script setup>
  import Logo from '@/assets/img/logo.png';
  import Roles from './RolesView.vue'
  </script>
  
  <style lang="scss" scoped></style>