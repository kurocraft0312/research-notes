<template lang="pug">
  div(class="container mx-auto px-4")
    div(class="flex content-center flex-wrap")
      div(v-for="article in articles" :key="article.key" class="w-1/3 p-4 max-w-sm rounded overflow-hidden shadow-lg")
        img(class="w-full" :src="article.eyecatch" alt="テスト")
        div(class="px-6 py-4")
          div(class="font-bold text-xl mb-2") {{article.title}}
          p(class="text-gray-700 text-base") {{article.description}}
        div(class="px-6 py-4")
          span(class="date") {{article.date}}
</template>
<script>
export default {
  data() {
    return {
      articles: [
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿1',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-19',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿2',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-20',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿3',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-21',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿4',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-22',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿5',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-23',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿6',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-24',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿7',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-25',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿8',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-26',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿9',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-27',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
        {
          eyecatch: '/test.jpg',
          title: 'テスト投稿10',
          description: 'これはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーんこれはテストだよーん',
          date: '2019-09-28',
          // category: life,
          // tag: human-life,
          // url: '/',
        },
      ]
    }
  }
}
</script>
