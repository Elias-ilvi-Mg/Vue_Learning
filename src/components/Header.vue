
    /* eslint-disable */
<template>
    <header>
        <h1>{{ title }}</h1>
        <Button 
            @toogle-add-task="$emit('toggle-add-task')"
            text="Add Task" 
            color="red" />
        <!-- <Button text="Update Task" color="black" /> -->
        <!-- <Button text="Remove Task" color="red" /> -->
    </header>
</template>

<script>
import Button from './Button.vue'

export default {
    name:'Header',
    props: {
        title: String,

    },
    components: {
        Button
    }
}
</script>

