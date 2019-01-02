<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container _mgbt-64px">
    <div class="row _jtfct-ct">
      <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-48px _pdbt-12px _fw-500 _mgbt-12px">
        งานของคุณ
      </div>
      <!-- If don't have current job -->
      <!-- <div class="col-12 _tal-ct _fs-5 _lh-125pct">
        ขณะนี้คุณยังไม่ได้รับงาน <br> คุณสามารถเลือกดูงานได้จากงานทั้งหมด
      </div> -->
      <!-- If have job(s) -->

      <div class="col-md-6 col-12">
      <active-card></active-card>
      </div>
      <div class="col-md-6 col-12">
      <active-card></active-card>
      </div>
      <div class="col-12 _pdv-12px _pdt-24px _tal-ct">
        <nuxt-link to="/dashboard/jobs/active" class=" _cl-red _fs-6  _cs-pt hover-underline-animation">
        ดูงานทั้งหมดของคุณขณะนี้
        </nuxt-link>
      </div>
      <div class="col-12 _w-100pct-md _w-50pct _bdbtw-1px _mgt-48px _bdcl-red"></div>

    </div>
    <div class="row _jtfct-ct">
      <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-48px _pdbt-12px _fw-500 _mgbt-12px">
        งานทั้งหมด
      </div>
        <div class="col-md-4 col-12">
          <urgent-card></urgent-card>
        </div>
        <div class="col-md-4 col-12">
          <urgent-card></urgent-card>
        </div>
        <div class="col-md-4 col-12">
          <job-card></job-card>
        </div>
        <div class="col-md-4 col-12">
          <job-card></job-card>
        </div>
        <div class="col-md-4 col-12">
          <upcoming-card></upcoming-card>
        </div>
        <div class="col-md-4 col-12">
          <upcoming-card></upcoming-card>
        </div>
      </div>
  </div>
</div>
</template>

<script>
import HeaderTH from '~/components/Header'
import urgentCard from '~/components/urgentCard'
import ActiveCard from '~/components/activeCard'
import jobCard from '~/components/jobCard'
import upcomingCard from '~/components/upcomingCard'
export default {
components: {
  HeaderTH,
  urgentCard,
  ActiveCard,
  jobCard,
  upcomingCard
}
}
</script>

<style>

</style>
