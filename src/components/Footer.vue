<template>
    <footer>
        <p>{{ t('farewell') }}</p>
    </footer>
</template>

<script setup lang="ts">
import { useI18n } from 'vue-i18n';

const { t } = useI18n();
</script>
