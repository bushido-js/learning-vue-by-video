<template>
    <li>
        {{todo.titel}}
    </li>
</template>

<script>
export default{
    props: {
        todo: {
            type: Object,
            required: true,
        }
    }
}

</script>

<!-- https://www.youtube.com/watch?v=OlnwgS-gk8Y
доделать -->