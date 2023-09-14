<template>
    <v-app>
        <v-main class="background-image">
            <Container />
        </v-main>
    </v-app>
</template>

<script setup>
    import Container from '@/components/Container.vue';
</script>

<style>
    :root {
        --teal: #00cebb;
    }

    body {
        margin: 0;
        padding: 0;

        width: 100vw;
        height: 100vh;
    }

    ::-webkit-scrollbar {
        width: .85vmin;
    }

    ::-webkit-scrollbar-track {
        background: rgb(20, 20, 20);
    }

    ::-webkit-scrollbar-thumb {
        border-radius: 5px;
        background: var(--teal);
    }

    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
    }

    .background-image {
        background-image: url('./assets/background.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center center;
    }
</style>
