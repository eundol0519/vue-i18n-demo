<template>
    <div>
        <h2>{{ t('home.title') }}</h2>
        <p>{{ t('home.description') }}</p>
        <input v-model="userName" :placeholder="t('inputPrompt')" />
        <p v-if="userName">{{ t('greeting') }}, {{ userName }}!</p>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import { useI18n } from 'vue-i18n';

const { t } = useI18n();

const userName = ref('');
</script>
