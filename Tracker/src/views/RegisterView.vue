<template>
    <section class="container-fluid" id="login-vue">
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
                                <input type="text" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Name" id="NameInput" />
                            </div>                           
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-at text-primary" xmlns="http://www.w3.org/2000/svg"
                                    width="24" height="24" fill="currentColor" viewBox="0 0 14 14">
                                    <path
                                        d="M13.106 7.222c0-2.967-2.249-5.032-5.482-5.032-3.35 0-5.646 2.318-5.646 5.702 0 3.493 2.235 5.708 5.762 5.708.862 0 1.689-.123 2.304-.335v-.862c-.43.199-1.354.328-2.29.328-2.926 0-4.813-1.88-4.813-4.798 0-2.844 1.921-4.881 4.594-4.881 2.735 0 4.608 1.688 4.608 4.156 0 1.682-.554 2.769-1.416 2.769-.492 0-.772-.28-.772-.76V5.206H8.923v.834h-.11c-.266-.595-.881-.964-1.6-.964-1.4 0-2.378 1.162-2.378 2.823 0 1.737.957 2.906 2.379 2.906.8 0 1.415-.39 1.709-1.087h.11c.081.67.703 1.148 1.503 1.148 1.572 0 2.57-1.415 2.57-3.643zm-7.177.704c0-1.197.54-1.907 1.456-1.907.93 0 1.524.738 1.524 1.907S8.308 9.84 7.371 9.84c-.895 0-1.442-.725-1.442-1.914z" />
                                </svg>

                                <!-- /svg -->
                                <input type="email" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Email" id="emailInput" />
                            </div>
                            <div class="mb-4 position-relative">
                                <!-- svg -->
                                <svg class="input-icon-start bi bi-emoji-smile text-primary"
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor"
                                    viewBox="0 0 16 16">
                                    <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z" />
                                    <path
                                        d="M4.285 9.567a.5.5 0 0 1 .683.183A3.498 3.498 0 0 0 8 11.5a3.498 3.498 0 0 0 3.032-1.75.5.5 0 1 1 .866.5A4.498 4.498 0 0 1 8 12.5a4.498 4.498 0 0 1-3.898-2.25.5.5 0 0 1 .183-.683zM7 6.5C7 7.328 6.552 8 6 8s-1-.672-1-1.5S5.448 5 6 5s1 .672 1 1.5zm4 0c0 .828-.448 1.5-1 1.5s-1-.672-1-1.5S9.448 5 10 5s1 .672 1 1.5z" />
                                </svg>
                                <!-- /svg -->
                                <input type="text" class="form-control form-control-lg rounded-0 shadow-sm ps-5"
                                    placeholder="Role" id="NameInput" />
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
                                <input type="password" class="form-control form-control-lg rounded-0 shadow-sm px-5"
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
                                <input type="password" class="form-control form-control-lg rounded-0 shadow-sm px-5"
                                    placeholder="Confirm Password" id="passwordInput" />
                            </div>

                            <div class="d-grid mb-4">
                                <button type="submit" class="btn btn-primary shadow-sm btn-lg rounded-0">
                                    Sign Up
                                </button>
                            </div>
                            <div class="text-center">
                                <div class="text-muted">Already have an account?</div>
                                <a href="#" class="text-decoration-none text-dark">Sign In</a>
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

.input-icon-end {
    position: absolute;
    right: 15px;
    top: 12px;
}
</style>
