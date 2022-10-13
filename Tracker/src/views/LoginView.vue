<template>
    <section class="container-fluid" id="login-vue">
        <div class="row d-flex justify-content-center align-items-center vh-100 bg-light">
            <div class="col-12 col-md-8 col-lg-4">
                <div class="card shadow-sm rounded-0">
                    <div class="card-body p-4 p-md-5 mx-md-4">
                        <div class="text-danger small">{{error}}</div>
                        <div class="mb-5">
                            <div class="display-6 mb-2 text-primary">Sign In</div>
                            <p class="text-muted">
                                To keep connected with us please login with your email address
                                and password. We will not share your information with others.
                            </p>
                        </div>
                        <form @submit.prevent="onSubmit">

                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-person text-primary"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path
                                        d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z" />
                                </svg>
                                <!-- /svg -->
                                <input type="email" v-model="email"
                                    class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="John@gmail.com" id="emailInput" />
                            </div>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-lock text-primary" xmlns="http://www.w3.org/2000/svg"
                                    width="24" height="24" fill="currentColor" viewBox="0 0 16 16">
                                    <path
                                        d="M8 1a2 2 0 0 1 2 2v4H6V3a2 2 0 0 1 2-2zm3 6V3a3 3 0 0 0-6 0v4a2 2 0 0 0-2 2v5a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V9a2 2 0 0 0-2-2zM5 8h6a1 1 0 0 1 1 1v5a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V9a1 1 0 0 1 1-1z" />
                                </svg>
                                <!-- /svg -->
                                <!-- svg -->
                                <svg class="input-icon-end bi bi-three-dots text-primary bg-light border"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path
                                        d="M3 9.5a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3zm5 0a1.5 1.5 0 1 1 0-3 1.5 1.5 0 0 1 0 3z" />
                                </svg>
                                <!-- /svg -->
                                <input type="password" v-model="password"
                                    class="form-control form-control-lg rounded-0 shadow-sm px-5" placeholder="******"
                                    id="passwordInput" />
                                <div class="mt-1 text-end">
                                    <router-link class="text-decoration-none mt-3 text-dark" to="/forgot-password">
                                        Forgot Password?</router-link>
                                </div>
                            </div>
                            <div class="mb-4 form-check">
                                <input type="checkbox" class="form-check-input" id="exampleCheck1" />
                                <label class="form-check-label" for="exampleCheck1">Remember me?</label>
                            </div>
                            <div class="d-grid mb-4">
                                <button v-on:click="signIn()" class="btn btn-primary shadow-sm btn-lg rounded-0">
                                    Sign In
                                </button>
                            </div>
                            <div class="text-center">
                                <div class="text-muted">Don't you have an account?</div>
                                <router-link class="text-decoration-none text-dark" to="/register">Sign Up</router-link>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import axios from "axios";
export default {
    data() {
        return {
            email: "",
            password: "",
            error: ""

        }
    },
    methods: {
        async signIn() {
            let result = await axios.get(`http://localhost:3000/user?email=${this.email}&password=${this.password}`);
            if (result.status == 200 && result.data.length > 0) {
                this.$router.push({ name: 'home' });
            }
            else {
                this.error = "Invalid Email & Password. Please try again :(";
            }
        },

    }
}

</script>
<style>
.input-icon-start {
    position: absolute;
    top: 12px;
    left: 15px;
}

.input-icon-end {
    position: absolute;
    right: 15px;
    top: 12px;
}
</style>
