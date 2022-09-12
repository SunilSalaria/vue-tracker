<template>
    <section class="container-fluid" id="register-vue">
        <div class="row d-flex justify-content-center align-items-center vh-100 bg-light">
            <div class="col-12 col-md-8 col-lg-4">
                <div class="card shadow-sm rounded-0">
                    <div class="card-body p-4 p-md-5 mx-md-4">
                        <div class="mb-5">
                            <div class="display-6 mb-2 text-primary">Sign Up</div>
                            <p class="text-muted">
                                To connect with us please fill below detail and then login.
                                We will not share your information with others.
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
                                <input type="text" v-model="name" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Name" id="nameInput" />
                            </div>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-at text-primary" xmlns="http://www.w3.org/2000/svg"
                                    width="24" height="24" fill="currentColor" viewBox="0 0 14 14">
                                    <path
                                        d="M13.106 7.222c0-2.967-2.249-5.032-5.482-5.032-3.35 0-5.646 2.318-5.646 5.702 0 3.493 2.235 5.708 5.762 5.708.862 0 1.689-.123 2.304-.335v-.862c-.43.199-1.354.328-2.29.328-2.926 0-4.813-1.88-4.813-4.798 0-2.844 1.921-4.881 4.594-4.881 2.735 0 4.608 1.688 4.608 4.156 0 1.682-.554 2.769-1.416 2.769-.492 0-.772-.28-.772-.76V5.206H8.923v.834h-.11c-.266-.595-.881-.964-1.6-.964-1.4 0-2.378 1.162-2.378 2.823 0 1.737.957 2.906 2.379 2.906.8 0 1.415-.39 1.709-1.087h.11c.081.67.703 1.148 1.503 1.148 1.572 0 2.57-1.415 2.57-3.643zm-7.177.704c0-1.197.54-1.907 1.456-1.907.93 0 1.524.738 1.524 1.907S8.308 9.84 7.371 9.84c-.895 0-1.442-.725-1.442-1.914z" />
                                </svg>

                                <!-- /svg -->
                                <input type="email" v-model="email" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Email" id="emailInput" />
                            </div>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-phone-flip text-primary"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path fill-rule="evenodd"
                                        d="M11 1H5a1 1 0 0 0-1 1v6a.5.5 0 0 1-1 0V2a2 2 0 0 1 2-2h6a2 2 0 0 1 2 2v6a.5.5 0 0 1-1 0V2a1 1 0 0 0-1-1Zm1 13a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1v-2a.5.5 0 0 0-1 0v2a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2v-2a.5.5 0 0 0-1 0v2ZM1.713 7.954a.5.5 0 1 0-.419-.908c-.347.16-.654.348-.882.57C.184 7.842 0 8.139 0 8.5c0 .546.408.94.823 1.201.44.278 1.043.51 1.745.696C3.978 10.773 5.898 11 8 11c.099 0 .197 0 .294-.002l-1.148 1.148a.5.5 0 0 0 .708.708l2-2a.5.5 0 0 0 0-.708l-2-2a.5.5 0 1 0-.708.708l1.145 1.144L8 10c-2.04 0-3.87-.221-5.174-.569-.656-.175-1.151-.374-1.47-.575C1.012 8.639 1 8.506 1 8.5c0-.003 0-.059.112-.17.115-.112.31-.242.6-.376Zm12.993-.908a.5.5 0 0 0-.419.908c.292.134.486.264.6.377.113.11.113.166.113.169 0 .003 0 .065-.13.187-.132.122-.352.26-.677.4-.645.28-1.596.523-2.763.687a.5.5 0 0 0 .14.99c1.212-.17 2.26-.43 3.02-.758.38-.164.713-.357.96-.587.246-.229.45-.537.45-.919 0-.362-.184-.66-.412-.883-.228-.223-.535-.411-.882-.571ZM7.5 2a.5.5 0 0 0 0 1h1a.5.5 0 0 0 0-1h-1Z" />
                                </svg>
                                <!-- /svg -->
                                <input type="text" v-model="phone" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Phone" id="phoneInput" />
                            </div>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-question-diamond text-primary"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path
                                        d="M6.95.435c.58-.58 1.52-.58 2.1 0l6.515 6.516c.58.58.58 1.519 0 2.098L9.05 15.565c-.58.58-1.519.58-2.098 0L.435 9.05a1.482 1.482 0 0 1 0-2.098L6.95.435zm1.4.7a.495.495 0 0 0-.7 0L1.134 7.65a.495.495 0 0 0 0 .7l6.516 6.516a.495.495 0 0 0 .7 0l6.516-6.516a.495.495 0 0 0 0-.7L8.35 1.134z" />
                                    <path
                                        d="M5.255 5.786a.237.237 0 0 0 .241.247h.825c.138 0 .248-.113.266-.25.09-.656.54-1.134 1.342-1.134.686 0 1.314.343 1.314 1.168 0 .635-.374.927-.965 1.371-.673.489-1.206 1.06-1.168 1.987l.003.217a.25.25 0 0 0 .25.246h.811a.25.25 0 0 0 .25-.25v-.105c0-.718.273-.927 1.01-1.486.609-.463 1.244-.977 1.244-2.056 0-1.511-1.276-2.241-2.673-2.241-1.267 0-2.655.59-2.75 2.286zm1.557 5.763c0 .533.425.927 1.01.927.609 0 1.028-.394 1.028-.927 0-.552-.42-.94-1.029-.94-.584 0-1.009.388-1.009.94z" />
                                </svg>
                                <!-- /svg -->
                                <input type="text" v-model="position" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Position" id="positionInput" />
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
                                <input type="password" v-model="password" class="form-control form-control-lg rounded-0 shadow-sm px-5"
                                    placeholder="Password" id="passwordInput" />
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
                                <input type="password" v-model="confirmPassword" class="form-control form-control-lg rounded-0 shadow-sm px-5"
                                    placeholder="Confirm Password" id="confirmPasswordInput" />
                            </div>
                            <div class="d-grid mb-4">
                                <button v-on:click="signUp()" class="btn btn-primary shadow-sm btn-lg rounded-0">
                                    Sign Up
                                </button>
                            </div>
                            <div class="text-center">
                                <div class="text-muted">Already have an account?</div>
                                <router-link class="text-decoration-none text-dark" to="/login">Sign In</router-link>
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
 export default{
     data(){
        return{
           name: "",
           email: "",
           phone: "",
           position: "",
           password: "",
           confirmPassword: ""
        }
     },
     methods:{
        async signUp(){            
        let result = await axios.post("http://localhost:3000/user", {
         name:this.name,
         email:this.email,
         phone:this.phone,
         position:this.position,
         password:this.password,
         confirmPassword:this.confirmPassword
        });        
        }
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
