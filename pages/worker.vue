<template>
  <div class="Worker">
    <h2 class="Worker-Heading">
      企業の皆様・はたらく皆様へ
    </h2>
    <div v-for="(item, i) in items" :key="i">
      <TextCard :title="item.title" :link="item.link" :body="item.body" />
    </div>
  </div>
</template>
<script lang="ts">
import TextCard from '@/components/TextCard.vue'
export default {
  components: {
    TextCard
  },
  data() {
    return {
      items: [
        {
          title: '新型コロナウイルス対策休業助成金制度',
          link:
            'https://www.pref.yamanashi.jp/koucho/coronavirus/info_coronavirus.html#rosei',
          body:
            'リンク先掲載の助成対象者に対して、休業した日、一人につき一日4,000円が助成されます。令和2年3月31日までの申請が必要です。'
        },
        {
          title: '子育て家庭休業助成金制度',
          link: 'https://www.pref.yamanashi.jp/koucho/coronavirus/info_coronavirus.html#josei',
          body:
            '子どもが小学校や保育所等へ登校・登園をしなかったことに伴い保護者が休業を余儀なくされた方に、一定額の助成を行うものです。'
        },
        {
          title: '経済変動対策融資（経済危機関係）',
          link:
            'https://www.pref.yamanashi.jp/koucho/coronavirus/documents/r020302keizaikiki.pdf',
          body:
            '1カ月間の売上高等が前年同月比で20％以上減少しており、かつ、その後の2カ月間を含む3カ月間の売上高等が前年同期比で20％以上の減少が見込まれる方が対象です。'
        },
        {
          title: '経済変動対策融資（不況業種対策関係）',
          link:
            'https://www.pref.yamanashi.jp/koucho/coronavirus/documents/r020306fukyougyousyu.pdf',
          body:
            '中小企業信用保険法第2条第5項第5号で指定する不況業種で、直近3カ月間の売上高等が前年同期比5%以上減少するなどしている方が対象です。'
        },
        {
          title: 'その他の融資',
          link:
            'https://www.pref.yamanashi.jp/shougyo/42590388393.html',
          body:
            'その他の融資についてはこちらをご覧ください。'
        },
        {
          title: '中小企業者等特別相談窓口',
          link: 'https://www.pref.yamanashi.jp/shouko-kik/koronasoudanmadoguchi.html',
          body:
            '県、商工会議所、商工会などの新型コロナウイルスに関する中小企業・小規模企業の相談窓口の一覧です。'
        }
      ]
    }
  },
  head() {
    return {
      title: '企業の皆様・はたらく皆様へ'
    }
  }
}
</script>
<style lang="scss">
.Worker {
  &-Heading {
    @include font-size(30);
    font-weight: normal;
    color: $gray-2;
    margin-bottom: 12px;
  }
}
a {
  @include text-link();
}
</style>
