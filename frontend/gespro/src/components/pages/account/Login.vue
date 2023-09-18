<template>
    <div class="login-container">
      <div class="login-form">
        <img :src="Logo" alt="Logo" class="logo" />
        <form @submit.prevent="login">
          <div class="mb-3 mt-4">
            <input v-model="username" type="text" class="form-control" placeholder="Usuario" />
          </div>
          <div class="mb-3">
            <input v-model="password" type="password" class="form-control" placeholder="Contraseña" />
          </div>
          <button class="btn btn-primary btn-block" type="submit">Iniciar Sesión</button>
        </form>
      </div>
      <div class="login-background">
        <img :src="BackgroundLogin" alt="BackgroundLogin" class="img-fluid" />
        <div class="slogan">
          Desde 1969, somos una empresa líder en construcción y gerencia de infraestructura.
        </div>
      </div>
    </div>
  </template>

<script setup>
  import Logo from '@/assets/img/logo.png';
  import BackgroundLogin from '@/assets/img/way1.jpg';
import { useRouter } from 'vue-router';
import { ref } from 'vue';

const router = useRouter();
const username = ref('');
const password = ref('');

const login = () => {
  if (username.value === '33333333' && password.value === '123456') {
    router.push('/dashboard'); 
  } else if (username.value === '12647847' && password.value === '123456') {
    router.push('/report');
  } else {
    console.error('Inicio de sesión fallido');
  }
};
</script>























  
  <style scoped>
  .login-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  .login-form {
    min-width: 300px;
    background-color: #fff;
    padding: 20px;
    text-align: center;
  }
  
  .logo {
    width: 120px;
  }
  
  .login-background {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }
  
  .slogan {
    position: absolute;
    color: #fff; /* Color de texto blanco */
    font-size: 28px;
    font-weight: bold;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Sombra de texto */
    animation: fadeIn 10s ease; /* Agregar animación de entrada */
  }
  
  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(-200px); /* Desplazamiento hacia arriba */
    }
    to {
      opacity: 1;
      transform: translateY(0); /* Posición normal */
    }
  }
  </style>
  
  