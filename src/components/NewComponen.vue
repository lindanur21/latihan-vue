<template>
    <div>
        <MyComponen nama="Linda" umur="17" jk="Perempuan" alamat="Sukamenak"></MyComponen>
        <LatihanComponen name="Linda" age="20"></LatihanComponen>
        <LatihanDuaComponen></LatihanDuaComponen>
        <WatchersComponen nama="Linda" umur="21"></WatchersComponen>
        <h2>Event Component</h2>
        <LatihanEventComponen :nama="nama" :umur="umur" @greeted="onGreeted">
            <template #footer>
                <div>
                    <p>Ini Adalah Footer Latihan Event</p>
                </div>
            </template>
            <template #header>
                    <div>
                        <p>Ini Adalah Header Latihan Event</p>
                    </div>
                </template>
        </LatihanEventComponen>
    </div>
</template>

<script setup>
//import MyHeader from './MyHeader.vue';
import LatihanEventComponen from '@/components/LatihanEventComponen.vue';
import MyComponen from './MyComponen.vue';
import LatihanComponen from './LatihanComponen.vue';
import LatihanDuaComponen from './LatihanDuaComponen.vue';
import WatchersComponen from './WatchersComponen.vue';

</script>
