<template>
  <div>
    <b-jumbotron>
      <template v-slot:header>Pufu&nbsp;<img :src="pufu_image" width="120"></template>
      <template v-slot:lead>
          すべての人にプロジェクトの体験を。     
      </template>
      <p>
          プロジェクトに携わる人に向けた<br>
          プロジェクト譜ツール
      </p>
      <b-button variant="outline-secondary" href="#">Pufuを利用する（準備中）</b-button>
    </b-jumbotron>
    <h2>Pufuの特徴</h2>
    <b-container class="bv-context-row">
      <b-row>
        <b-col>
          <b-card title="プロジェクトの可視化" class="mb-2 context-card">
            <p>プロジェクトを譜面で表現することで、プロジェクトの状況や関係性を把握</p>
          </b-card>
        </b-col>
        <b-col>
          <b-card title="メンバー共有" class="mb-2 context-card">
            <p>プロジェクトへのメンバー登録ができ、編集したプロジェクト譜をWebでいつでもメンバーに共有</p>
          </b-card>
        </b-col>
        <b-col>
          <b-card　title="ポータビリティ" class="mb-2 context-card">
            <p>PCブラウザに加えてモバイルブラウザーに対応し、場所を問わずプロジェクト譜を編集、閲覧</p>
          </b-card>
        </b-col>
      </b-row>
      <h3>Pufuのプラン</h3>
      <b-row class="justify-content-md-center">
        <b-col md="4">
          <b-card no-body bg-variant="default" header="フリープラン" class="text-center">
            <b-list-group>
              <b-list-group-item>
                <b>プロジェクト作成</b><br>
                5プロジェクトまで
              </b-list-group-item>
              <b-list-group-item>
                <b>共有可能ユーザー</b><br>
                3ユーザー/1プロジェクト
              </b-list-group-item>
              <b-list-group-item>
                <b>参加可能プロジェクト</b><br>
                無制限
              </b-list-group-item>
            </b-list-group>
          </b-card>
        </b-col>
      </b-row>
      <h3>動作端末</h3>
      <b-row class="justify-content-md-center">
        <b-col md="6">
          <b-card no-bdy bg-variant="default">
            <b-list-group horizontal>
              <b-list-group-item class="flex-fill">
                <p>
                  <b>PC ブラウザ<br>(Windows 10)</b>
                </p>
                <img :src="chrome_image"/>
                <p>Chrome</p>
              </b-list-group-item >
              <b-list-group-item class="flex-fill">
                <p>
                  <b>モバイルブラウザ<br>(iOS)</b>
                </p>
                <img :src="safari_image"/>
                <p>Safari</p>
              </b-list-group-item>
            </b-list-group>
          </b-card>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <h3>プロジェクト譜に興味がある方</h3>
          <b-card
            title=""
            img-alt="book"
            img-top
            tag="article"
            style="max-width: 30rem;"
            class="mb-2 book"
          >
            <div class="amazlet-box" style="margin-bottom:0px;"><div class="amazlet-image" style="float:left;margin:0px 12px 1px 0px;"><a href="http://www.amazon.co.jp/exec/obidos/ASIN/4883354377" name="amazletlink" target="_blank"><img src="https://images-fe.ssl-images-amazon.com/images/I/51JLRdl-IsL._SL160_.jpg" alt="予定通り進まないプロジェクトの進め方" style="border: none;" /></a></div><div class="amazlet-info" style="line-height:120%; margin-bottom: 10px"><div class="amazlet-name" style="margin-bottom:10px;line-height:120%"><a href="http://www.amazon.co.jp/exec/obidos/ASIN/4883354377" name="amazletlink" target="_blank">予定通り進まないプロジェクトの進め方</a><div class="amazlet-powered-date" style="font-size:80%;margin-top:5px;line-height:120%">posted with <a href="http://www.amazlet.com/" title="amazlet" target="_blank">amazlet</a> at 19.11.09</div></div><div class="amazlet-detail">前田考歩 後藤洋平 <br />宣伝会議 (2018-03-29)<br />売り上げランキング: 6,267<br /></div><div class="amazlet-sub-info" style="float: left;"><div class="amazlet-link" style="margin-top: 5px"><a href="http://www.amazon.co.jp/exec/obidos/ASIN/4883354377" name="amazletlink" target="_blank">Amazon.co.jpで詳細を見る</a></div></div></div><div class="amazlet-footer" style="clear: left"></div></div>
          </b-card>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          Powered by <a href="https://dyson-yamashita.github.io/winkry-site/">Winkry</a>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
export default {
  name: 'Top',
  data() {
    return {
      pufu_image: require("../assets/pufu_image.png"), 
      safari_image: require("../assets/safari.png"),
      chrome_image: require("../assets/chrome.png") 
     }
  }
}
</script>
<style scoped>
.row {
  margin: 20px 0px 40px 0px;
}
.context-card {
  padding: 0px 20px 0px 20px;
  max-width: 30rem;
}
.book {
  margin: auto;
}
</style>