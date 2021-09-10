<script setup  lang="ts">
 const msg="nihao"
 import { defineProps, reactive } from "vue";
    const props = defineProps({
    email: String
    });
</script>

<template>
    <div>
        <p> 我的名称：{{msg}}</p>
        <p> 邮箱：{{email}}</p>
    </div>
</template>