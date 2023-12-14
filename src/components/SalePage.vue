<template>
    <div class="sale">
        <h2>
            Our Products
        </h2>

        <div class="product">
            <div class="cart">
                <img src="../assets/image2.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

            <div class="cart">
                <img src="../assets/image1.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

            <div class="cart">
                <img src="../assets/image3.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

            <div class="cart">
                <img src="../assets/image4.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

            <div class="cart">
                <img src="../assets/image5.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

            <div class="cart">
                <img src="../assets/image6.jpg" alt="">
                <div class="cartbtn">
                    <button @click="cartBtn">View Cart</button>
                    <button @click="cartBtn">Add To Cart</button>
                </div>
            </div>

        </div>


    </div>
</template>

<script>
export default {
    methods: {
        cartBtn(){
            alert('this feature is yet to be added')
        }
    }
};
</script>

<style>
.sale {
    margin: 80px 0;
    width: 100%;
    display: grid;
    place-items: center;
}

.sale h2 {
    font-size: 24px;
    margin-bottom: 20px;
}

.product {
    display: grid;
    grid-template-columns: auto auto auto;
    place-items: center;
    gap: 50px 30px;
    width: 1100px;
}

.product img {
    width: 340px;
    box-shadow: 0 0 4px 0 #d1d0d0;
}

.cart{
    position: relative;
    overflow: hidden;
    transition: .2s;
}
.cartbtn{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgb(0, 0, 0, .3);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 30px;
    z-index: 9;
    opacity: 0;
    visibility: hidden;
    transition: .3s ease-out;
    margin-top: -5px;
}
.cart:hover .cartbtn{
    opacity: 1;
    visibility: visible;
}
.cartbtn:hover{
    opacity: 1;
    visibility: visible;
}
.cartbtn button{
    border: none;
    padding: 13px 23px;
    border-radius: 6px;
    background: #f7f7f7;
    font-family: sans-serif;
    transition: .2s ease;
}
.cartbtn button:hover{
     background: #000;
     color: #fff;
}
button{
    cursor: pointer;
}
@media screen and (max-width:900px){
    .product {
    display: grid;
    grid-template-columns: auto auto;
    place-items: center;
    gap: 50px 30px;
    width: 85%;
    }
}

@media screen and (max-width:768px){
    .product{
    gap: 50px 10px;
    width: 100%;
    }
}

@media screen and (max-width:500px){
    .product {
    display: grid;
    grid-template-columns: auto;
    place-items: center;
    gap: 50px 30px;
    width: 85%;
}
}
@media screen and (max-width:350px){
    .product img{
        width: 300px;
    }
}
</style>