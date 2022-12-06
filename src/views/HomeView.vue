<template lang="pug">
#home
  img(:src="bear")
  br
  br
  p
    |小熊維尼難得一本正經
    br
    |手上拿著一張紙
    br
    |表情微微皺眉、面露不悅
    br
    |我到底看了什麼？
    br
    |維尼圖支援
</template>

<script setup>
// 如果圖片 src 是綁定本機圖片，不能直接寫路徑
// const principal = '@/assets/0104.jpg'
const bear = new URL('@/assets/123.jpg', import.meta.url).href
</script>
