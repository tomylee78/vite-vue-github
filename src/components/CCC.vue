<script>
    export default{
        data(){
            return {
                CCC: "我是C",
            };
        },
        props: ["bbb", "aaa"],
    }
</script>

<template>
  <div>{{ bbb }}，{{ CCC }}{{ `。我則是從最外部傳來的 => ${aaa}` }}</div>
</template>
