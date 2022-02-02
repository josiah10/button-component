<template>
    <div>
        <div class="container">
           <h2>Buttons</h2>
            <div class="flx first">
                <Buttons box="0px 2px 3px rgba(51, 51, 51, 0.2)" tex="Default" color="#3F3F3F" text="<Button />" textColor="#333333" bgColor="#E0E0E0" bord="none"/>
                <Buttons box="0px 2px 3px rgba(51, 51, 51, 0.2)" tex="Default" color="#3F3F3F" text="&:hover, &:focus" textColor="#828282" bgColor="#AEAEAE" bord="none"/>
            </div>
            <div class="flx second">
                <Buttons tex="Default" color="#3D5AFE" text="<Button variant=”outline” />" textColor="#333333" bgColor="white" bord="1px solid #3D5AFE"/>
                <Buttons tex="Default" color="#3D5AFE" text="&:hover, &:focus" textColor="#828282" bgColor="#2962FF1A" bord="1px solid #3D5AFE"/>
            </div>

            <div class="flx third">
                <Buttons tex="Default" color="#3D5AFE" text="<Button variant=”text” />" textColor="#333333" bgColor="#FFFFFF" bord="none"/>
                <Buttons tex="Default" color="#3D5AFE" text="&:hover, &:focus" textColor="#828282" bgColor="#2962FF1A" bord="none"/>
            </div>

            <div class="flx third">
                <Buttons tex="Default" color="#FFFFFF" text="<Button disableShadow />" textColor="#333333" bgColor="#3D5AFE" bord="none"/>
            </div>

            <div class="flx Four">
                <Buttons tex="Disabled" color="#9E9E9E" text="<Button disabled />" textColor="#000000" bgColor="#E0E0E0" bord="none"/>
                <Buttons tex="Disabled" color="#9E9E9E" text="<Button variant=”text” disabled />" textColor="#333333" bgColor="#FFFFFF" bord="none"/>
            </div>

            <div class="flx Five">
                <Buttons box="0px 2px 3px rgba(0, 49, 202, 0.2)" class="fiv" sou="cart-plus" tex="Default" color="#FFFFFF" text="<Button startIcon=”local_grocery_store” />" textColor="#000000" bgColor="#2962FF" bord="none"/>
                <Buttons box="0px 2px 3px rgba(0, 49, 202, 0.2)" sour="cart-plus" tex="Default" color="#FFFFFF" text="<Button startIcon=”local_grocery_store” />" textColor="#000000" bgColor="#2962FF" bord="none"/>

            </div>
                <i class="fa fa-cart-plus"></i>
            <div class="flx six">
                <div>
                    <p>{{text2}}</p>
                    <button class="sm">Default</button>
                </div>
                <Buttons box="0px 2px 3px rgba(0, 0, 0, 0.2)" tex="Default" color="#FFFFFF" text="<Button size=”md” />" textColor="#000000" bgColor="#2962FF" bord="none"/>
                <div>
                    <p>{{text1}}</p>
                    <button class="lg">Default</button>
                </div>
            </div>

            <div class="flx six">
                <Buttons box="0px 2px 3px rgba(51, 51, 51, 0.2)" tex="Default" color="#3F3F3F" text="<Button color=”default” />" textColor="#000000" bgColor="#E0E0E0" bord="none"/>
                <Buttons box=" 0px 2px 3px rgba(41, 98, 255, 0.2)" tex="Default" color="#FFFFFF" text="<Button size=”md” />" textColor="#000000" bgColor="#2962FF" bord="none"/>
                <Buttons box=" 0px 2px 3px rgba(69, 90, 100, 0.2)" tex="Secondary" color="#FFFFFF" text="<Button color=”secondary” />" textColor="#000000" bgColor="#455A64" bord="none"/>
                <Buttons box="0px 2px 3px rgba(211, 47, 47, 0.2)" tex="Danger" color="#FFFFFF" text="<Button color=”danger” />" textColor="#000000" bgColor="#D32F2F" bord="none"/>
            </div>

            <div class="flx last">
                <Buttons box="0px 2px 3px rgba(51, 51, 51, 0.2)" tex="Default" color="#3F3F3F" text="&:hover, &:focus" textColor="#828282" bgColor="#AEAEAE" bord="none"/>
                <Buttons box=" 0px 2px 3px rgba(41, 98, 255, 0.2)" tex="Default" color="#FFFFFF" text="ffff" textColor="#FFFFFF" bgColor="#0039CB" bord="none"/>
                <Buttons box=" 0px 2px 3px rgba(69, 90, 100, 0.2)" tex="Secondary" color="#FFFFFF" text="ff" textColor="#FFFFFF" bgColor="#1C313A" bord="none"/>
                <Buttons box="0px 2px 3px rgba(211, 47, 47, 0.2)" tex="Danger" color="#FFFFFF" text="fff" textColor="#FFFFFF" bgColor="#9A0007" bord="none"/>
            </div>
            <h4>Icons: https://material.io/resources/icons/?style=round</h4>
            <h5>created by <span>Josiah</span> - devChallenges.io</h5>
        </div>

    </div>
</template>

<script>
    import Buttons from "./Buttons";
    export default {
        name: "Rightside",
        data(){
            return{
              text1:"<Button size=”lg” />",
                text2:"<Button size=”sm” />"
            }
        },
        components:{
            Buttons
        }
    }
</script>

<style scoped>
    .container{
        padding: 53px 0 0 320px;
    }
    h2 {
        font-family: Poppins;
        font-style: normal;
        font-weight: 500;
        font-size: 24px;
        line-height: 36px;
        color: #4F4F4F;
    }
    .flx{
        display: flex;
        align-items: start;
        flex-direction: row;
        margin-bottom: 40px;
    }
    .sm{
        font-family: Noto Sans;
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 20px;
        text-align: center;
        border-radius: 6px;
        margin-right: 150px;
        padding: 6px 12px;
        background: #2962FF;
        color: #FFFFFF;
        border: none;
        box-shadow: 0 2px 3px rgba(0, 49, 202, 0.2);
    }
    .lg{
        font-family: Noto Sans;
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 20px;
        text-align: center;
        border-radius: 6px;
        margin-right: 150px;
        padding: 11px 22px;
        background: #2962FF;
        color: #FFFFFF;
        border: none;
        box-shadow: 0px 2px 3px rgba(0, 49, 202, 0.2);
    }
    p{
        font-family: Ubuntu Mono;
        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 12px;
        margin-bottom: 12px;
        color: #000000;
    }
    h4{
        font-family: Ubuntu Mono;
        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 12px;
        color: #828282;
        margin-bottom: 34px;
    }
    h5 {
        font-family: Montserrat;
        font-style: normal;
        font-weight: 500;
        font-size: 14px;
        line-height: 17px;
        color: #A9A9A9;
    }
    h5 span{
        font-weight: 600;
        text-decoration: underline;
    }
    .fiv{
        padding-right: 77px;
    }


</style>