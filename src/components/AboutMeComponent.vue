<template>
    <div class="container ">
        <div class="row">
            <div id="profilePhoto" class=" col-md-4">
                <img src="../assets/profile.jpg" style="width: 100%">
            </div>
            <div class="col-md-8" >
                <h1 style="text-align: left;">About me</h1>
                <p>I work as software developer and IT analyst in most italian famous sofa seller.<br />
                    Lorem ipsum dolor sit amet, quo ei simul congue exerci, ad nec admodum perfecto
                            mnesarchum, vim ea mazim fierent detracto. Ea quis iuvaret expetendis his, te elit voluptua
                            dignissim
                            per, habeo iusto primis ea eam.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
addEventListener('resize', (event) => {
    let el = document.getElementById('profilePhoto');
    if(window.innerWidth > 768) {
        el.classList.remove('order-last');
    }else{
        el.classList.add('order-last');
    }
});

onresize = (event) => {};

</script>
<style>
.center {
    text-align: center;
}
.justify {
    text-align: justify;
}

</style>