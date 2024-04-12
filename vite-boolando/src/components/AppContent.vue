<template>
        <main>
            <section class="section">
                <div class="container">
                    <div class="flex row">
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/1.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-red">-50%</span>
                                    <span class="second-badge badge bg-green">Sostenibilità</span>
                                    <div class="overlay">
                                        <img src="/1b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Levi's</p>
                                    <h4>RELAXED FIT TEE UNISEX</h4>
                                    <p><span class="red">14,99&euro;</span><span class="line-throught">29,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/2.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-red">-30%</span>
                                    <div class="overlay">
                                        <img src="/2b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Guess</p>
                                    <h4>ROSES TEE</h4>
                                    <p><span class="red">20,99&euro;</span><span class="line-throught">29,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/3.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-red">-30%</span>
                                    <div class="overlay">
                                        <img src="/3b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Come Zucchero Filato</p>
                                    <h4>VOGLIA DI COLORI PASTELLO</h4>
                                    <p><span class="red">129,99&euro;</span><span class="line-throught">184,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/4.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-red">-50%</span>
                                    <span class="second-badge badge bg-green">Sostenibilità</span>
                                    <div class="overlay">
                                        <img src="/4b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Levi's</p>
                                    <h4>TEE UNISEX</h4>
                                    <p><span class="red">14,99&euro;</span><span class="line-throught">29,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/5.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <div class="overlay">
                                        <img src="/5b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Maya Deluxe</p>
                                    <h4>STRIPE BODICE</h4>
                                    <p><span class="red">99,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                        <div class="col-3">
                            <div class="card">
                                <div class="card-image">
                                    <img src="/6.webp" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-green">Sostenibilità</span>
                                    <div class="overlay">
                                        <img src="/6b.webp" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>Esprit</p>
                                    <h4>MAGLIONE - BLACK</h4>
                                    <p><span class="red">29,99&euro;</span></p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </main>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss">
.card-image{
    position: relative;
}
.card-image > img{
    display: block;
}
.badge{
    line-height: 20px;
    color: white;
    font-size: 10px;
    padding: 0 5px;
}
.card{
    padding: 15px;
}
.card-image .badge {
    position: absolute;
    bottom: 35px;
    z-index: 10;
    left: 0px;
}
.card-image .second-badge{
    left: 40px
}
.heart-icon{
    position: absolute;
    right: 0px;
    top: 10px;
    z-index: 10;
    line-height: 35px;
    padding: 0 8px;
    font-size: 28px;
    background-color: white;
}
.card-image .overlay{
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    opacity: 0;
    transition: none;
}
.card:hover .overlay{
    opacity: 1;
}
</style>