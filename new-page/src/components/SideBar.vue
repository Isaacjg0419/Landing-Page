<template>
    <div>
        <div class="sideBar " style="height:auto;width:100%">
            <div  v-if='isShow' @click='close' class="blur " style="padding:0px;">
            </div>
            <div v-if='isShow' class="content text-start" style="min-width: 350px;background-color:black;height: 100%;">
                <div class="row">
                    <div class="col">
                        <div class="row" style="width:100%">
                            <div class="col-auto text-start" style="padding:10px 20px">
                                <img style="height:10vh;width: 10vw;" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/logo-new@2x.png">
                            </div>
                            <div class="col text-end my-auto">
                                <button class='close' @click='close' style="border:none;background-color: black;color: white;">X</button>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col" style="padding:15px 30px;">
                                HOME
                            </div>
                        </div>
                        <div class="row">
                            <div class="col" style="padding:15px 30px;">
                                ABOUT US
                            </div>
                        </div>
                        <div class="row">
                            <div class="col" style="padding:15px 30px;">
                                Service
                            </div>
                        </div>
                        <div class="row">
                            <div class="col" style="padding:15px 30px;">
                                PAGES
                            </div>
                        </div>
                        <div class="row">
                            <div class="col" style="padding:15px 30px;">
                                CONTACT US
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script type="text/javascript">
export default {
    name: 'SideBar',
    props: ['SideBar'],
    data() {
        return {
            isShow: true,

        }
    },
    methods: {

        close() {
            this.isShow = false;

            this.$emit('closeSidebarEvent')
            console.log(this.isShow)

        },
    },

}
</script>
<style scoped>
.content {
    color: white;
    position: fixed;
    z-index: 9999;
    right: 0;
}

.blur {

    height: 100%;
    width: 100%;
    opacity: 0.6;
    background-color: #515151;
    position: fixed;

    z-index: 9998;

}
</style>