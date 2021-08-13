<template>
    <li>
        todo item 1
    </li>
</template>

<script>
export default {
   props: {
       todo: {
           type: Object,
           required: true
       }
   }
}
</script>
