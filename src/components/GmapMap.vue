<template>
    <GmapMap
        :center="{lat:7.3692, lng:5.1193}"
        :zoom="7"
        map-type-id="roadmap"
        style="width: 500px; height: 300px"
        >
        <GmapMarker
            :key="index"
            v-for="(m, index) in markers"
            :position="m.position"
            :clickable="true"
            :draggable="true"
            @click="center=m.position"
        />
    </GmapMap>
</template>