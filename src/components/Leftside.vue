<template>
    <div class="left">
        <div class="container">
            <h3><span>Dev</span>challenges.io</h3>
            <ul class="list">
                <li>Colors</li>
                <li>Typography</li>
                <li>Spaces</li>
                <li>Buttons</li>
                <li class="active">Inputs</li>
                <li>Grid</li>
             </ul>
      </div>
    </div>
</template>

<script>
    export default {
        name: "Leftside"
    }
</script>

<style scoped>
    .left{
       position: absolute;
        width: 237px;
        height: 1234px;
        left: -8.5px;
        top: -9.07px;
        background: #FAFBFD;
    }
    .container{
        padding: 47.5px 0 0 56.5px;
    }
    h3{
        font-family: Poppins;
        font-style: normal;
        font-weight: 600;
        font-size: 13px;
        line-height: 19px;
        margin-bottom: 122px;
    }
    h3 span{
        color: #F7542E;
    }
    .list{
        list-style: none;
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        flex-direction: column;
        padding-left: 0;
    }
    li{
        font-family: Noto Sans;
        font-weight: 500;
        font-size: 14px;
        font-style: normal;
        line-height: 20px;
        color: #9E9E9E;
        padding-bottom: 35px;
        cursor: pointer;
    }
    .active{
        font-weight: bold;
        color: #090F31;
    }
</style>