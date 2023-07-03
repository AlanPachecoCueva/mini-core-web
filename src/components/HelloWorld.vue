<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

    <el-date-picker v-model="startDate" class="datePicker" format="DD/MM/YYYY" value-format="DD/MM/YYYY"
      type="date" placeholder="Fecha De Conclusión Estimada"></el-date-picker>

    <el-date-picker v-model="endDate" class="datePicker" format="DD/MM/YYYY" value-format="DD/MM/YYYY"
      type="date" placeholder="Fecha De Conclusión Estimada"></el-date-picker>

    <button @click="handleClick">Haz clic</button>


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
        return {
          startDate: "",
          endDate: "",
        }
    },
    methods: {

    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
