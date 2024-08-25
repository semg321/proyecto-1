<script lang="ts" setup>

defineProps({
    name:String,
    type:String
})

</script>


<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
            <h4 class="card-title">{{ name }}</h4>
            <h5 class="card-text">{{ type }}</h5>
        </div>
        <div class="card-body">
            <a href="#" class="card-link">Conectar</a>
        </div>
    </div>
</template>