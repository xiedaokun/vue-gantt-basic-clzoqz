<template>
  <DefaultTheme>
    <Gantt :tasks="tasks" :links="links" :scales="scales" :columns="columns" />
  </DefaultTheme>
</template>

<script>
  import { Gantt, DefaultTheme } from "@dhtmlx/trial-vue-gantt";
  import { columns, scales, tasks, links } from "./data";

  export default {
    name: "App",
    components: {
      Gantt, DefaultTheme
    },
    data: () => ({
      columns,
      scales,
      tasks,
      links
    })
  };
</script>