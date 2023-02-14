<script>
    import BBB from './BBB.vue'
    export default{
        data(){
            return {
                AAA: "我是A",
            };
        },
        components:{
            BBB,
        },
        methods:{
            get_event(){
                console.log("由內部元件觸發");
            }
        },
    }
</script>

<template>
    <div>
        <BBB :aaa="AAA" @click_event="get_event"></BBB>
    </div>
</template>