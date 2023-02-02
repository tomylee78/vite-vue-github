<script>
    export default{
        data(){
            return {
                CCC: "你好",
            };
        },
        props: ["url"],
    }
</script>

<template>
  <div>{{ url }}，{{CCC}}</div>
</template>
