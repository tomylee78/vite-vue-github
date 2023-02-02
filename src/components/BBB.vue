<script>
    export default{
        data(){
            return {
                CCC: "你好",
            };
        },
        props: ["ttt"],
    }
</script>

<template>
  <div>{{ ttt }}，{{CCC}}</div>
</template>
