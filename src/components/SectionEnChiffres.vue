<template>
    <div class="mt-5">&nbsp;</div>

    <h2 class="text-3xl md:text-4xl lg:text-5xl mt-4 mx-auto text-center font-bold couleur-rose">
        <span class="couleur-bleue">Neopass</span> En Chiffres
    </h2>
    
    <div class="sm:flex  w-full justify-around">
        <div class="counter">
            <div class="box">
                <i class="fas fa-user-graduate"></i>
                <div class="num">13</div>
                Structures utilisatrices
            </div>
        </div>
    
        <div class="counter">
            <div class="box">
                <i class="fas fa-user-graduate"></i>
                <div class="num">1149</div>
                Passeports créés
            </div>
        </div>
    
        <div class="counter">
            <div class="box">
                <i class="fas fa-user-graduate"></i>
                <div class="num">487</div>
                Plans d'accompagnements
            </div>
        </div>
    </div>

</template>

<script setup>
    $(document).ready(function(){
        $('.num').counterUp({
        time: 3000
        });
    });
</script>


<style>
    .counter-sec{
    padding: 80px 0;
    width: 100%;
    background: #131416;
    position: absolute;
    top: 50%;
    width: 100%;
    transform: translateY(-50%);
    }
    .num{
    font-size: 50px;
    margin: 20px 0;
    }
    .box{
    flex: 1;
    text-align: center;
    padding: 20px;
    color: #3524c8;
    text-transform: uppercase;
    }
    .box i{
    font-size: 50px;
    color: #333;
    }
</style>