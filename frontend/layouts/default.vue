<template lang="pug">
  //- header
  div(class="head-menu")
    nav(class="flex items-center justify-between flex-wrap bg-teal-500 p-6")
      div(class="flex items-center flex-shrink-0 text-white mr-6")
        svg(class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg")
          path(d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z")
        span(class="font-semibold text-xl tracking-tight") ggrks-life
      div(class="block lg:hidden")
        button(class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white")
          svg(class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg")
            title Menu
              path(d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z")
      div(class="w-full block flex-grow lg:menu-bar lg:items-center lg:w-auto")
        div(v-for="menu in menus" :key="menu.key" class="text-sm")
          a(:href="menu.url" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4") {{menu.title}}
    //- contents
    div(class="container mx-auto px-4")
      div(class="flex content-center flex-wrap")
        div(v-for="article in articles" :key="article.key" class="lg:w-1/3 md:w-1/2 p-4 rounded overflow-hidden shadow-lg")
          img(class="w-full" :src="article.eyecatch" alt="テスト")
          div(class="px-6 py-4")
            div(class="font-bold text-xl mb-2") {{article.title}}
            p(class="text-gray-700 text-base") {{article.description}}
          div(class="px-6 py-4")
            span(class="date") {{article.date}}
    //- sidebar
    div(class="flex content-center flex-wrap")

</template>
<style lang="scss">
.text-sm {
  display: inline;
}
@media (min-width: 1024px) {
  .lg\:menu-bar {
    text-align: right;
  }
}
</style>
<script>
export default {
  data() {
    return {
      menus: [
        {
          title:'HOME',
          url: '/',
        },
        {
          title:'ABOUT',
          url: '/about',
        },
        {
          title:'CONTACT',
          url: '/contact',
        },
      ],
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
