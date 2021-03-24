<template>
    <div id="app">
        <compBookListOne></compBookListOne>
        <compBookListTwo></compBookListTwo>
        <button class="btn btn-warning" @click="reducePrice">Reduce Price</button>
    </div>
</template>

<script>
import compBookListOne from "./components/BookListOne"
import compBookListTwo from "./components/BookListTwo"
export default {
    data(){
        return{
            
        }
    },
    components:{
      compBookListOne,
      compBookListTwo
    },
    methods: {
        reducePrice(){
            this.$store.dispatch("reducePrice");
        }
    }
}
</script>
