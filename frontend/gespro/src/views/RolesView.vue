<template>
    <div class="container-fluid">
        <div class="row d-flex justify-content-center">
            <nav class="col-12 justify-content-start  ">
                <a class="btn btn-secondary btn-sm m-4" href="#" aria-current="page">Crear Usuario</a>
            </nav>
            <div class="row">
                <div class="col-2">
                    <div class="card m-2">
                        <div class="card-header">
                            <h5>Crear Usuario</h5>
                        </div>
                        <div class="card-body">
                            <form @submit.prevent="crearUsuario">
                                <div class="mb-3">
                                    <label for="nombre" class="form-label">Nombre</label>
                                    <input type="text" class="form-control" id="nombre" v-model="nombre" required>
                                </div>
                                <div class="mb-3">
                                    <label for="email" class="form-label">Correo Electrónico</label>
                                    <input type="email" class="form-control" id="email" v-model="email" required>
                                </div>
                                <div class="mb-3">
                                    <label for="password" class="form-label">Contraseña</label>
                                    <input type="password" class="form-control" id="password" v-model="password" required>
                                </div>
                                <div class="mb-3">
                                    <label for="departamento" class="form-label">Departamento</label>
                                    <select class="form-select" id="departamento" v-model="departamento" required>
                                        <option value="ventas">Ventas</option>
                                        <option value="marketing">Marketing</option>
                                        <option value="tecnologia">Tecnología</option>
                                        <!-- Agrega más opciones de departamentos según sea necesario -->
                                    </select>
                                </div>
                                <div class="mb-3">
                                    <label for="rol" class="form-label">Perfil</label>
                                    <select class="form-select" id="rol" v-model="rol" required>
                                        <option value="admin">Admin</option>
                                        <option value="usuario">Usuario</option>
                                        <!-- Agrega más opciones de roles según sea necesario -->
                                    </select>
                                </div>
                                <div class="text-center">
                                    <button type="submit" class="btn btn-success btn-sm w-75">Crear Usuario</button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
                <div class="col-10">
                    <div class="table m-2">
                        <table class="table table-sm">
                            <thead>
                                <tr>
                                    <th scope="col" style="background-color: #dddddd;">ID</th>
                                    <th scope="col" style="background-color: #dddddd;">Nombre</th>
                                    <th scope="col" style="background-color: #dddddd;">Email</th>
                                    <th scope="col" style="background-color: #dddddd;">Departamento</th>
                                    <th scope="col" style="background-color: #dddddd;">Perfil</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>

                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>


                                <tr class="">
                                    <th scope="col">U001</th>
                                    <th scope="col">Luis Caraballo</th>
                                    <th scope="col">Admin@hyhcolombia.com</th>
                                    <th scope="col">Tecnología</th>
                                    <th scope="col">Administrador</th>
                                </tr>
                                <tr class="">
                                    <th scope="col">ID</th>
                                    <th scope="col">Nombre</th>
                                    <th scope="col">Email</th>
                                    <th scope="col">Departamento</th>
                                    <th scope="col">Perfil</th>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const rol = ref('');
const permiso = ref('acceso_total');

const crearPerfil = () => {
    if (!rol.value || !permiso.value) {
        console.error('Por favor, complete todos los campos.');
        return;
    }

    // Aquí puedes agregar la lógica para crear el perfil de acceso
    console.log('Perfil creado:', { rol: rol.value, permiso: permiso.value });
};
</script>

<style lang="scss" scoped></style>