<template>
    <div>
        <h2>{{ t('about.title') }}</h2>
        <p>{{ t('about.description') }}</p>
    </div>
</template>

<script setup lang="ts">
import { useI18n } from 'vue-i18n';

const { t } = useI18n();
</script>
