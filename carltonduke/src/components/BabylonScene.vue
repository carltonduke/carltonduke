<template>
    <canvas ref="bjsCanvas" width="500" height="500" />
</template>

<script setup>
    import { ref, onMounted } from "@vue/runtime-core";
    import { createScene } from "../scenes/MyFirstScene";

    // Reference to the canvas element
    const bjsCanvas = ref(null);

    // Lifecycle hook to initialize the scene
    onMounted(() => {
    if (bjsCanvas.value) {
        createScene(bjsCanvas.value);
    }
    });
</script>