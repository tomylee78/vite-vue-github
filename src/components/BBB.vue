<script>
    import CCC from "./CCC.vue";
    export default{
        data(){
            return {
                BBB: "我是B",
                TTT: "",
            };
        },
        components:{
            CCC,
        },
        props: ["aaa"],
        methods:{
            event_trigger(){
                console.log("我要向外呼叫你囉~");
                this.$emit("click_event");
            }
        },
    }
</script>

<template>
  <div>{{ aaa }}，</div>
  <CCC :bbb="BBB" :aaa="aaa"></CCC>
  <button @click="event_trigger">我是按鈕</button>
</template>
