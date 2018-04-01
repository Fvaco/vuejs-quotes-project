<template>
    <div class="row">
        <app-quote @click.native="deleteQuote(index)" v-for="(quote, index) in quotes">
            {{ quote }}
        </app-quote>
    </div>
</template>

<script>
    import Quote from './Quote.vue'
    export default {
        props: ['quotes'],
        methods:{
            deleteQuote(index){
                this.$emit("quoteDeleted", index);
            }
        },
        components:{
            appQuote: Quote
        }
    }
</script>

<style scoped>

</style>