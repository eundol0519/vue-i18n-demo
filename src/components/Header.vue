<template>
    <header>
        <h1>{{ t('greeting') }}</h1>
        <button @click="changeLang('ko')">한국어</button>
        <button @click="changeLang('en')">English</button>
    </header>
</template>

<script setup lang="ts">
import { useI18n } from 'vue-i18n';

const { t, locale } = useI18n();

function changeLang(lang: 'ko' | 'en') {
    locale.value = lang;
}
</script>
