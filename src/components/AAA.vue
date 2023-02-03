<script>
    import BBB from './BBB.vue'
    export default{
        data(){
            return {
                text1: "你好",
            };
        },
        components:{
            BBB,
        }
    }
</script>

<template>
    <div>
        <BBB :ttt="text1"></BBB>
    </div>
</template>