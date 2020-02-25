<template>
  <div class="fielderFrame">
    <div>
      <ul>
        <li class="number" v-for="number in 9" :key="number">{{number}}番</li>
      </ul>
    </div>

    <div>
      <draggable tag="ul">
        <li class="fielder" v-for="fielder in 9" :key="fielder">
          <div>
            ポジション : <Selectbox />
          </div>
          <div>
            選手名 : <input type="text">
          </div>
        </li>
      </draggable>
    </div>
  </div>
</template>

<script>
  import "@/assets/css/fielder.css"
  import draggable from 'vuedraggable'
  import Selectbox from '@/components/selectbox'

  export default {
    components: { 
      draggable,
      Selectbox
    },
  }
</script>
