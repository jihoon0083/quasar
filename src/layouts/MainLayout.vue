<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

        <q-toolbar-title> Quasar App </q-toolbar-title>

        <q-btn flat round dense icon="light_mode" />
        <!--
          dark_mode
        -->
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      <q-list>
        <q-item-label header>
          <q-avatar class="q-mr-sm" size="xl">
            <!--
            <img src="/icons/favicon-96x96.png" />
            -->
            <img src="https://i.mydramalist.com/QYwJg_5c.jpg" />
          </q-avatar>
          <span> Quasar v{{ $q.version }}</span>
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>
<script>
const linksList = [
  {
    title: 'Typography',
    caption: 'quasar.dev',
    icon: 'school',
    to: '/typography',
  },
  {
    title: 'Colors',
    caption: 'quasar.dev',
    icon: 'school',
    to: '/colors',
  },
  {
    title: 'Spacing',
    caption: 'quasar.dev',
    icon: 'school',
    to: '/spacing',
  },
  {
    title: 'BrakePoint',
    caption: 'quasar.dev',
    icon: 'school',
    to: '/brakepoint',
  },
  {
    title: 'Classes & Variables',
    caption: 'quasar.dev',
    icon: 'school',
    to: '/classes-variables',
  },
];
</script>

<script setup>
import { defineComponent, ref } from 'vue';
import EssentialLink from 'components/EssentialLink.vue';

const leftDrawerOpen = ref(false);
const essentialLinks = linksList;
const toggleLeftDrawertoggleLeftDrawer = () =>
  (leftDrawerOpen.value = !leftDrawerOpen.value);
</script>
