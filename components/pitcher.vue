<template>
  <div class="pitcherFrame">
    <ul>
      <li class="pitcher" v-for="pitcher in pitchers" v-bind:key="pitcher.id">
        <div>{{pitcher.name}}</div>
        <div>
          選手名 : <input type="text">
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
  import "@/assets/css/pitcher.css"
  import draggable from 'vuedraggable'

  export default {
    components: {},
    data() {
      return {
        pitchers: [
          {id: 1, name: "　先発　"},
          {id: 2, name: "中継ぎ１"},
          {id: 3, name: "中継ぎ２"},
          {id: 4, name: "中継ぎ３"},
          {id: 5, name: "　抑え　"}
        ]
      }
    }
  }
</script>
