<template>
    <div class="conatainer">
        <div class="row">
            <div class="col-md-4">
            <ul>
                <li v-for="hobby in hobbies" :key="hobby">{{hobby}}</li>
            </ul>
            </div>
        </div>
    </div>
</template>

<script>
     export default{
         data() {
             return {
                 hobbies:['Swimming','Travelling', 'Series']
             }
         },
     }

</script>