<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container">
    <div class="row">
      <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-48px _pdbt-12px _fw-500">
        งานของคุณ
      </div>
      <div class="col-12 _tal-ct _fs-5">
        ขณะนี้คุณยังไม่ได้รับงานคุณสามารถเลือกดูงานได้ 
        <nuxt-link to="/"><span class="_cl-red hover-underline-animation-red">ที่นี่</span></nuxt-link>
      </div>
      <div class="col-12 _w-100pct _bdbtw-1px _mgt-48px _bdcl-neutral-500"></div>
    </div>
    <div class="row _jtfct-ct">
      <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-48px _pdbt-12px _fw-500">
        งานทั้งหมด
      </div>
      <div class="col-md-10 col-6 _bgcl-white box-shadow _tal-ct _fs-5">
        ขณะนี้คุณยังไม่ได้รับงานคุณสามารถเลือกดูงานได้ 
        <nuxt-link to="/"><span class="_cl-red hover-underline-animation-red">ที่นี่</span></nuxt-link>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import HeaderTH from '~/components/Header'
export default {
components: {
  HeaderTH
}
}
</script>

<style>

</style>
