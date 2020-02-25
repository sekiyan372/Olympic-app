<template>
  <section>
    <div class="title">ぼくのかんがえたさいきょうのさむらいじゃぱん</div>
    <div class="warning">
      <ul>
        <li>※ 選択できる選手は2020年の東京オリンピック出場資格を持った選手だけです。</li>
        <li>※ 打順はドラッグ&ドロップで切り替えることができます。</li>
      </ul>
    </div>
    <div class="main">
      <Fielder />
      <Pitcher />
    </div>
  </section>
</template>

<script>
  import "@/assets/css/index.css"
  import Fielder from "@/components/fielder"
  import Pitcher from "@/components/pitcher"

  export default {
    components: {
      Fielder,
      Pitcher
    }
  }
</script>
