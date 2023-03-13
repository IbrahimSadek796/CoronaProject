<template>
    <section class="transmission py-5 mt-5" id="transmission">
        <div class="container">
            <div class="main-title">
                <h2 class="mb-3">transmission of covid-19</h2>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eaque, at error! Dolorem, saepe dolorum error ut esse vel, asperiores animi perspiciatis itaque cum placeat ratione aspernatur dicta odio fugiat minima.</p>
            </div>
            <div class="row">
                <div class="col-md-4">
                    <div class="box bg-body rounded shadow my-5">
                        <div class="image">
                            <img src="../../assets/image/spread-a.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Person-to-Person spread as close contact with infacted</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="box bg-body rounded shadow my-5">
                        <div class="image">
                            <img src="../../assets/image/spread-b.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Touching our contact with infacted surfaces of objacts</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="box bg-body rounded shadow my-5">
                        <div class="image">
                            <img src="../../assets/image/spread-c.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Droplets that from infacted person coughs or sneezes</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="link text-center mt-5">
                <a href="#" class=" btn btn-outline-primary text-light bg-primary"><i class="bi bi-question-circle me-2"></i>  Have question about spreading?</a>
            </div>
        </div>
    </section>
</template>


<style scoped>
.main-title h2::before{
    content: "How coronavirus is spread";
}
.transmission .row .box .image img{
    width: 100%;
}
.transmission .row .box .info{
    border-top: 5px solid #0077b6;
    padding: 10px;
}
.transmission .row .box .info h5{
    color: var(--main-color);
}
.transmission .container > .link .btn{
    border-radius: 20px !important;
    margin-top: 20px;
}
</style>