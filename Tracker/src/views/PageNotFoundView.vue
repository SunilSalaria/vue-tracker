<script setup>

</script>

<template>
 <section class="container-fluid" id="error-vue">
    <div class="row d-flex justify-content-center align-items-center vh-100">
            <div class="col-12 col-md-8 col-lg-4">
                <div class="card border-0">
                    <div class="card-body text-center">
                        <div class="mb-4 mx-md-5">
                            <div class="display-3 mb-2 text-primary fw-bold">404</div>
                            <div class="display-6 mb-2 text-primary">Page not Found</div>
                            <p class="text-muted">
                                The link you clicked may be broken or the page may have been removed or renamed.
                            </p>
                        </div>  
                        <div>
                        <img src="../assets/img/illustration.png" class="img-fluid" alt="...">   
                        </div>       
                        <div>
                        <router-link class="btn btn-primary shadow-sm btn-lg rounded-0" to="/home">Go to Home</router-link>                        
                        </div>           
                    </div>
                </div>
            </div>
        </div>   
 </section>
</template>

<style>
    
</style>