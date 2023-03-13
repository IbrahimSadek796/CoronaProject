<template>
    <section class="treatment py-5" id="treatment">
        <div class="overlay"></div>
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <div class="main-title py-5 my-5 text-white">
                        <h2 class="mb-3">treatment for coronavirus</h2>
                        <p class="text-light"><span>to date, there is no vaccine and no specific antiviral madicin to prevent or treat COVID-2019. </span>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Obcaecati nobis quo explicabo sint assumenda? Saepe accusantium, ratione qui suscipit debitis tempore temporibus facere aspernatur odio.</p>

                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, consequatur repellendus architecto illum laboriosam tempora suscipit excepturi aliquam vel beatae blanditiis obcaecati, a magnam quisquam repudiandae sapiente quibusdam harum nobis adipisci error fugit? Quis ipsum qui autem sunt, dolor earum.</p>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="box py-5 my-5">
                        <h6>Salf care</h6>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta eaque voluptates eos maxime, perspiciatis nam!</p>
                        <span><i class="bi bi-arrow-right-short fs-2 fw-bold"></i>Lorem, ipsum dolor.</span>
                        <span><i class="bi bi-arrow-right-short fs-2 fw-bold"></i>Lorem, ipsum.</span>
                        <span><i class="bi bi-arrow-right-short fs-2 fw-bold"></i>Lorem ipsum dolor sit.</span>
                        <span><i class="bi bi-arrow-right-short fs-2 fw-bold"></i>Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque, quaerat.</span>
                        <h6>Medical Treatment</h6>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, alias! Officia laborum quia quidem nam mollitia obcaecati quo, praesentium odio?</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.treatment {
    background-image: url(../../assets/image/shape-a.png);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    color: #fff;
}
.treatment .overlay{
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 256, .5);
    z-index: 0;
}
.treatment .container{
    position: relative;
}
.treatment .container .main-title p{
    font-weight: 600;
    text-align: left;
    margin-bottom: 20px;
}
.main-title h2{
    color: #fff;
    font-size: 25px;
    margin-left: 0%;
    text-align: left;
}
.main-title h2::before{
    content: "be carefull & stay safe";
    color:aqua;
    text-align: left;
}
.treatment .container .main-title span{
    font-weight: bold;
}
.treatment .container .box {
    background-color: rgb(17, 17, 116);
    padding: 10px;
    width: auto;
}
.treatment .container .box span{
    display: flex;
    justify-content: left;
    align-items: center;
    position: relative;
    
}
.treatment .container .box span:last-of-type{
    margin-bottom: 5px;
}
.treatment .container .box span i{
    
    top: 0;
}
</style>