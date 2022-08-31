<template>
    <section class="container-fluid" id="login-vue">
        <div class="row d-flex justify-content-center align-items-center vh-100 bg-light">
            <div class="col-12 col-md-8 col-lg-3">
                <div class="card shadow-sm rounded-5">
                    <div class="card-body p-md-4">
                    <div class="text-center mb-5">
                        <img class="" src="../assets/tracker-index-logo.svg"
                                height="100" alt="index-logo-img">
                    </div>
                        
                <div class="display-6 mb-5 text-center">Sign In Now</div>
                <form>
                    <div class="mb-4">
                        <input type="email" class="form-control form-control-lg rounded-pill shadow-sm" id="emailInput">
                    </div>
                    <div class="mb-4">
                        <input type="password" class="form-control form-control-lg rounded-pill shadow-sm"
                            id="passwordInput">
                    </div>
                    <div class="mb-4 form-check">
                        <input type="checkbox" class="form-check-input" id="exampleCheck1">
                        <label class="form-check-label" for="exampleCheck1">Check me out</label>
                    </div>                    
                    <div class="d-grid mb-4 pt-5 mt-md-5">
                        <button type="submit" class="btn btn-primary shadow-sm btn-lg rounded-pill">Sign In</button>
                    </div>
                    <div class="text-center">
                        <div class="text-muted">Don't you have an account?</div>
                    <a href="#" class="text-decoration-none">Sign Up</a>
                    </div>
                    
                </form>
                </div>
                </div>
            </div>
        </div>
    </section>
</template>



<style>
</style>
