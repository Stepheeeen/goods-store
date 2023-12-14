<template>
    <div class="hero">
        <div class="description">
        <h2>Welcome to Charity Store.</h2>
        <p>No 1 rated store in Nigeria.</p>
        <button>Explore</button>
        </div>
        
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
    .hero{
        margin-top: 80px;
        width: 100%;
        height: 550px;
        background: url('../assets/hdr.png') no-repeat;
        background-position: right;
        background-size: contain;
        display: grid;
        align-items: center;
        padding: 10px;
        font-family: sans-serif;
    }
    .description{
        margin-top: -150px;
        margin-left: 30px;
    }
    .description h2{
        font-size: 45px;
    }
    .description p{
        font-size: 16px;
        line-height: 35px;
    }
    .description button{
        padding: 9px 18px;
        border: none;
        background: #1858b1;
        color: white;
        border-radius: 5px;
        box-shadow: 0 0 7px 0 #b1b0b0;
        margin-top: 5px;
    }

    @media screen and (max-width: 900px){
        .hero{
            background-color: rgb(177, 176, 176, .2);  
            padding: 0;
        }
        .description{
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            gap: 20px;
            margin-top: 5px;
            opacity: 1;
            width: 100%;
            height: 100%;
            background: rgb(177, 176, 176, .4);
            margin-left: 0;
        }
        .description p{
            font-size: 31px;
            font-weight: 600;
        }
    }

    @media screen and (max-width: 500px){
        .description h2{
            font-size: 30px;
        }
        .description p{
            font-size: 21px;
            font-weight: 600;
        }
    }
</style>