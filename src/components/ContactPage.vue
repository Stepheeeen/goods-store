<template>
    <div class="footer">
        <div class="subscribe">
            <input type="text" placeholder="Subscribe to our Newsletter" v-model="newsLetter">
            <button @click="submitBtn" type="submit">Submit</button>
        </div>
        
        <div class="contact">
            <p>Contact us at example@email.com</p>
        </div>
    </div>
</template>

<script>
    export default{
        data() {
            return {
                newsLetter: ''
            };
        },
        methods: {
            submitBtn(){
                const input = this.newsLetter;
                if(input == ''){
                    alert('please input your email')
                } else{
                    alert('you have subscribed successfully')
                }
            },
        }
    };
</script>

<style>
    .footer{
        display: grid;
        place-items: center;
        width: 100%;
        /* position: fixed; */
        bottom: 0;
        left: 0;
        height: 350px;
        background: #010f22;
    }
    .subscribe{
        margin-bottom: -170px;
    }
    .subscribe input{
        width: 270px;
        height: 35px;
        padding: 10px;
        border: none;
    }
    .subscribe button{
        margin-left: 10px;
        height: 38px;
        border: none;
        margin-top: 2px;
        width: 70px;
        border-radius: 3px;
        color: white;
        background: #1858b1;
    }
    .contact{
        font-size: 16px;
        margin-bottom: -20px;
        color: white;
    }
</style>