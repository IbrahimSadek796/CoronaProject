<template>
    <section class="prevention py-5 mt-5" id="prevention">
        <div class="container">
            <div class="main-title">
                <h2 class="mb-3">prevention & advice</h2>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eaque, at error! Dolorem, saepe dolorum error ut esse vel, asperiores animi perspiciatis itaque cum placeat ratione aspernatur dicta odio fugiat minima.</p>
            </div>
            <div class="row">
                <div class="col-md-3">
                    <div class="box my-5">
                        <div class="image">
                            <img src="../../assets/image/advice-a.png" alt="">
                        </div>
                        <div class="info">
                            <h5>What your hands frequently</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="box my-5">
                        <div class="image">
                            <img src="../../assets/image/advice-b.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Maintain social distancing</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="box my-5">
                        <div class="image">
                            <img src="../../assets/image/advice-c.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Avoid touching face</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-3">
                    <div class="box my-5">
                        <div class="image">
                            <img src="../../assets/image/advice-d.png" alt="">
                        </div>
                        <div class="info">
                            <h5>Practice respiratory hygience</h5>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora ducimus porro vitae officia nulla provident sunt in nostrum natus repellat?</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="link text-center mt-5">
                <a href="#steps" class=" btn btn-outline-primary text-light bg-primary me-3">Check how you wash hand <i class="bi bi-arrow-right-short fs-2 fw-bold ms-3"></i></a>
                <a href="#question" class=" btn text-primary">Q&A on Coronavirus <i class="bi bi-arrow-right-short fs-2 fw-bold ms-3"></i></a>
            </div>
        </div>
    </section>
</template>


<style scoped>
.main-title h2::before{
    content: "How coronavirus is spread";
}
.prevention .row .box {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.prevention .row .box .image img{
    width: 100px;
    height: 100px;
    border-radius: 50%;
}
.prevention .row .box .info{
    
    padding: 10px;
}
.prevention .row .box .info h5{
    color: var(--main-color);
}
.prevention .container > .link {
   display: flex;
   align-items: center;
   justify-content: center;
   
}
.prevention .container > .link .btn{
    border-radius: 30px !important;
    margin-top: 20px;
   display: flex;
   align-items: center;
   width: fit-content;
   justify-content: center;
   flex-direction: row;
}
@media (max-width: 767px) {
    .prevention .container > .link {
        flex-direction: column;
        
     }
     .prevention .container > .link .btn{
         border-radius: 30px !important;
         margin-top: 20px;
        display: flex;
        align-items: center;
        width: fit-content;
        justify-content: center;
        flex-direction: row;
     }
}
</style>