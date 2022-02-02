<template>
    <div>
        <p :style="{color:textColor}">{{text}}</p>
        <button :style="{background:bgColor,border:bord,color:color}"><span ><fa class="lef" :icon="sou" /></span>{{tex}}<span ><fa class="rig" :icon="sour" /></span></button>
    </div>
</template>


<script>
    export default {
        name: "Buttons",
        props:{
            text:String,
            textColor:String,
            bgColor:String,
            bord:String,
            color:String,
            tex:String,
            sou:String,
            sour:String

        }
    }
</script>

<style scoped>
    p{
        font-family: Ubuntu Mono;
        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 12px;
        margin-bottom: 12px;
    }
    button{
        padding: 8px 16px;
        font-family: Noto Sans;
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 20px;
        text-align: center;
        border-radius: 6px;
        margin-right: 150px;
    }
    .lef{
        padding-right: 10.13px;
    }
    .rig{
        padding-left: 10.13px;
    }

</style>