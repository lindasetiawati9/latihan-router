<template>
  <center>
  <h1>Detail {{ detail.nama }}</h1>
  <img :src="getImgSrc(detail.img)" alt="Category Image" />
  <h4>Harga : {{ detail.harga }}</h4>
</center>
</template>
<script>
import { produk } from '@/assets/Produk'

export default {
  props: [
      "id_produk"
  ],
  setup(props)
  {
      const detail = produk["produk"].find(function (item) {
          return item.id == props.id_produk;
      });

      const getImgSrc = (imgFileName) => {
    return '../src/assets/img/' + imgFileName + '';
   };
      return {
          detail,
          getImgSrc
      }
  }
}
</script>

<style>
  img {
    height: 150px;
  }
</style>