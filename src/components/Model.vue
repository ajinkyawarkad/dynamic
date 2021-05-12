<template>
    <div class="model">
        <div>Model Dialog</div>
        <div>
            <button @click.prevent="hideModel">ok</button>
        </div>
        
    </div>
</template>

<script>


export default {
    methods: {
        hideModel(){
            this.$emit('close')

        }
    },
   
}
</script>


