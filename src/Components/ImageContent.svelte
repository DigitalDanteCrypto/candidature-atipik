<script>
    
    // This declares a 'src' prop that can be passed in from the parent component
  export let src = ''; 
</script>

<div id="img-container">
    <img {src}alt="">
</div>



<style>

/* MOBILE */

@media screen and (min-width: 320px){
    #img-container {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 2rem;
    margin-bottom: 4rem;
}


img {
    padding: 1rem;
    object-fit: cover;
    border-radius: 2rem;
    max-width: 100%;
}


}



/* DESKTOP */

@media screen and (min-width: 1024px){


#img-container {
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 2rem;
    margin-bottom: 4rem;
}


img {
    height: 28rem;
    object-fit: cover;
    border-radius: 2rem;
    max-width: 100%;
}
}

</style>