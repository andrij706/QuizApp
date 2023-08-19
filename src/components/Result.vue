<script setup>
    import {defineProps} from 'vue'
    import {RouterLink} from 'vue-router'

    const {quizQuestionLenght, numberOfCorrectAnswers} = defineProps(['quizQuestionLenght', 'numberOfCorrectAnswers'])
</script>

<template>
    <div class="results">
        <p>Your Resulys...</p>
        <h1>
            {{numberOfCorrectAnswers }}/{{ quizQuestionLenght }}
        </h1>
        <RouterLink to="/">Go Back</RouterLink>
    </div>
</template>

<style scoped>
    .results{
        text-align: center;
        padding: 100px 0;
    }

    p {
        font-size: 25px;
    }

    h1 {
        font-size: 80px;
    }
</style>