<template>
    <section class="container-fluid" id="forgot-vue">
        <div class="row d-flex justify-content-center align-items-center vh-100 bg-light">
            <div class="col-12 col-md-8 col-lg-4">
                <div class="card shadow-sm rounded-0">
                    <div class="card-body p-4 p-md-5 mx-md-4">
                        <div class="mb-5">
                            <div class="display-6 mb-2 text-primary">Sign In</div>
                            <p class="text-muted">
                                To keep connected with us please login with your email address
                                and password. We will not share your information with others.
                            </p>
                        </div>
                        <form>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-person text-primary"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path
                                        d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z" />
                                </svg>
                                <!-- /svg -->
                                <input type="email" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Email" id="emailInput" />
                            </div>                           
                            <div class="d-grid mb-4">
                                <button type="submit" class="btn btn-primary shadow-sm btn-lg rounded-0">
                                    Submit
                                </button>
                            </div>
                            <div class="text-center">
                                <div class="text-muted">Back to Sign In</div>
                                <router-link class="text-decoration-none text-dark" to="/login">Sign In</router-link>         
                              </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style>
.input-icon-start {
    position: absolute;
    top: 12px;
    left: 15px;
}

.input-icon-end{
    position: absolute;
    right: 15px;
    top: 12px;
}
</style>
