<template>
    <v-container>
        <v-row class="d-flex flex-column justify-center fadeonrender">
            <v-col v-for="link in mediaLinks" :key="link.name" cols="auto">
                <v-btn
                    class="linkbutton"
                    color="primary"
                    variant="outlined"
                    :href="link.url"
                    min-width="330"
                    rel="noopener noreferrer"
                    size="large"
                    target="_blank"
                    :aria-label="link.name"
                >
                    <v-icon :icon="link.icon" size="large" start /> {{ link.name }}
                </v-btn>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        data() {
            return {
                mediaLinks: [
                    {
                        name: 'Twitter',
                        url: 'https://twitter.com/alex_arizola',
                        icon: 'mdi-twitter'
                    },
                    {
                        name: 'Instagram',
                        url: 'https://instagram.com/alex.arizola/',
                        icon: 'mdi-instagram'
                    },
                    {
                        name: 'Threads',
                        url: 'https://threads.net/@alex.arizola',
                        icon: 'mdi-dots-circle'
                    },
                    {
                        name: 'Portfolio',
                        url: 'https://alexarizola.dev/',
                        icon: 'mdi-card-account-details'
                    },
                    {
                        name: 'LinkedIn',
                        url: 'https://linkedin.com/in/alexander-arizola/',
                        icon: 'mdi-linkedin'
                    },
                    {
                        name: 'GitHub',
                        url: 'https://github.com/GhostDaGhost',
                        icon: 'mdi-github'
                    },
                    {
                        name: 'Email',
                        url: 'mailto:alexarizola46@gmail.com',
                        icon: 'mdi-email'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    .linkbutton {
        color: var(--teal) !important;
        border-color: var(--teal);
    }

    .fadeonrender {
        opacity: 0;
        animation: fadeIn .4s ease-in-out 2s forwards;
    }
</style>
