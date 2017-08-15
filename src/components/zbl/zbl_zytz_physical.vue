<template>
<div class="zbl_zytz_physical" style="overflow-x:hidden;background-color:#fff;height:100vh;">
    <iframe :src="physicalSrc" width="100%" height="100%"></iframe>
    <!-- <a :href="physicalSrc"></a> -->
</div>
</template>
<script>
export default {
    data: function() {
        return {
            physicalSrc: ''
        }
    },
    computed: {},
    components: {},
    methods: {},
    created() {},
    mounted() {
        // this.physicalSrc = require(`./zbl_physical/physical_${this.$route.query.typeId}.html`)
    }
}
</script>
<style lang='stylus' scoped>
mainColor = #35B46F
greyFont = #ADADAD
fontSize = .4rem
.header {
    position: fixed;
    width: 100%;
    height: auto;
    z-index: 11;
    .mint-header {
        height: 1rem;
        font-size: fontSize;
        background-color: mainColor;
    }
}
.body {
    position: absolute;
    top: 1rem;
    left: 0;
    right: 0;
    .itemList {
        display: flex;
        flex-direction: row;
        align-items: center;
        font-size: .35rem;
        padding: 10px 0 10px 20px;
        border-bottom: 1px solid #ddd;
        .avatar {
            width: 1.2rem;
            height: 1.2rem;
        }
        .text {
            margin: 0 20px;
            line-height: 1.5;
        }
        .rightOr {
            .right {
                display: inline-block;
                padding: .1rem;
                text-align: center;
                color: #fff;
                background-color: red;
                border-radius: 100%;
            }
            .perhepsRight {
                display: inline-block;
                padding: .1rem;
                text-align: center;
                color: #fff;
                background-color: red;
                border-radius: 100%;
            }
        }
        .link {
            position: absolute;
            right: 0;
            margin-right: 10px;
            span {
                font-size: .3rem;
                color: grey;
            }
            img {
                 width: .2rem;
                 height: .2rem;
                 margin-left: 8px;
            }
        }
    }
}
</style>
