<template>
  <div id="app">
      <table>
        <tr>
          <td>编号</td>
          <td>书名</td>
          <td>作者</td>
        </tr>
        <tr v-for="i in books" :key="i.id">
          <td>{{i.id}}</td>
          <td>{{i.name}}</td>
          <td>{{i.author}}</td>
        </tr>
      </table>
  </div>
</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      books:[
        {
         id:1,
         name:'java',
          author:'小王'
        },
        {
          id:2,
          name:'vue',
          author:'小李'
        },
        {
          id:3,
          name:'Spring Boot',
          author:'小明'
        }
    ]
      }
    }

  }

</script>

<style>

</style>
