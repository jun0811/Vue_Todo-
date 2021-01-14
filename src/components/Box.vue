<template>
  <div>
      <div v-bind:class="['box', color]" 
      v-bind:style = "{width: width+'px', height: height +'px'}"></div>
  </div>
</template>

<script>
export default {
    props: {
      color: { type : String, default: ""}  
    },
    data(){
        return{
            width : 40,
            height : 80
        }}
}
</script>

<style scoped>
    .box{
        border: 1px solid #000;
    }
    .blue {
        background : #009bff
    }
    .purple {
        background : purple
    }
    .green {
        background : green
    }
</style>