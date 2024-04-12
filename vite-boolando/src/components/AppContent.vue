<template>
        <main>
            <section class="section">
                <div class="container">
                    <div class="flex row">
                        <div class="col-3"
                        v-for="product in products"
                        >
                            <div class="card">
                                <div class="card-image">
                                    <img :src="'/'+ product.frontImage" alt="">
                                    <span class="heart-icon">&hearts;</span>
                                    <span class="badge bg-red">-50%</span>
                                    <span class="second-badge badge bg-green">Sostenibilità</span>
                                    <div class="overlay">
                                        <img :src="'/'+ product.backImage" alt="">
                                    </div>
                                </div>
                                <div>
                                    <p>{{product.brand}}</p>
                                    <h4>{{product.name}}</h4>
                                    <p><span class="red">{{product.price}}&euro;</span><span class="line-throught">29,99&euro;</span></p>
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
        data() {
            return {
                "products": [
    {
      "id": 1,
      "frontImage": "1.webp",
      "backImage": "1b.webp",
      "brand": "Levi's",
      "name": "Relaxed Fit",
      "price": 29.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 2,
      "frontImage": "2.webp",
      "backImage": "2b.webp",
      "brand": "Guess",
      "name": "Roses Tee",
      "price": 20.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "discount",
          "value": "-30%"
        }
      ]
    },
    {
      "id": 3,
      "frontImage": "3.webp",
      "backImage": "3b.webp",
      "brand": "Come Zucchero Filato",
      "name": "Voglia di colori pastello",
      "price": 129.99,
      "isInFavorites": false,
      "badges": [
        {
          "type": "discount",
          "value": "-30%"
        }
      ]
    },
    {
      "id": 4,
      "frontImage": "4.webp",
      "backImage": "4b.webp",
      "brand": "Levi's",
      "name": "Tee Unisex",
      "price": 14.99,
      "isInFavorites": false,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 5,
      "frontImage": "5.webp",
      "backImage": "5b.webp",
      "brand": "Maya Deluxe",
      "name": "Stripe Bodice",
      "price": 99.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 6,
      "frontImage": "6.webp",
      "backImage": "6b.webp",
      "brand": "Esprit",
      "name": "Maglione - Black",
      "price": 29.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        }
      ]
    }
  ]
            }
        },
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