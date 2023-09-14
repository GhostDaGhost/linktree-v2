<template>
    <v-container class="text-white text-center py-10 mb-12">
        <Logo />
        <Name />
        <Bio />
        <Links />
    </v-container>
</template>

<script setup>
    import Name from '@/components/Name.vue';
    import Logo from '@/components/Logo.vue';
    import Links from '@/components/Links.vue';
    import Bio from '@/components/Bio.vue';
</script>
