<script>
export default {
    
}
</script>
<template>
    <header class="bg-white pt-3">
        <div class="container d-flex align-items-center justify-content-between">
            <img src="../assets/dc-logo.png" alt="DC Logo" class="me-3">
            <nav class="flex-grow-1">
                <ul class="nav justify-content-end me-5" style="margin-right: 20%;">
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Characters</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Comics</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Movies</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">TV</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Games</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Collectibles</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Videos</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Fans</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">News</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link text-uppercase text-dark" href="#">Shop</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<style lang="scss">
      nav{
        font-weight: bold;
       }
       .nav-link {
        font-weight: bold;
        position: relative;
        transition: color 0.3s;
    }
    
    .nav-link::after {
        content: '';
        position: absolute;
        width: 0;
        height: 5px;
        display: block;
        margin-top: 50px;
        right: 0;
        background: #0383f9;
        transition: width 0.3s ease;
    }
    
    .nav-link:hover {
        color: #0383f9;
    }
    
    .nav-link:hover::after {
        width: 100%;
        left: 0;
        background: #0383f9;
    }
    
</style>