<template>
    <div>
        <h1>vue-timer-hook </h1>
        <p>Current Time Demo</p>
        <div>
            <span>{{time}}</span><span>{{time.hours}}</span>:<span>{{time.minutes}}</span>:<span>{{time.seconds}}</span><span>{{time.ampm}}</span>
        </div>
    </div>
</template>


<script lang="ts">
import { defineComponent } from "vue";
import { useTime } from 'vue-timer-hook';

export default defineComponent({
  name: "Home",
  setup() {
    const format = '24-hour'
    const time = useTime(format);
    return {
        time,
     };
  },
});
</script>

