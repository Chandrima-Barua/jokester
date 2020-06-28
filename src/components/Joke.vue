<template>
    <div class="col-md-6">
    <div class="joke-card">
    <div class="card-block">
    <button class="close" @click="removeJoke(index)"><span>&times;</span></button>
    <p><u>{{jokes.setup}}</u></p>
    <p><em>{{jokes.punchline}}</em></p>
    </div>
    </div>
    </div>
</template>
<script>
import {mapActions} from 'vuex'

export default {
    props:['jokes', 'index'],
    methods:mapActions([
        
        'removeJoke'
        
    ]),
}
</script>