<template>
    <div>
        <div class="row">
            <div class="col-sm-12">
                <h3>Quotes Added</h3>
                <div class="progress">
                    <div class="progress">
                        <div class="progress-bar"
                             role="progressbar"
                             :style="{width: (quotesCount/maxQuotes) * 100 + '%'}">
                            {{ quotesCount }} / {{ maxQuotes }}
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        props: ['quotesCount', 'maxQuotes']
    }
</script>

<style scoped>

</style>