<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container">
    <div class="row _jtfct-ct _mgt-48px">
    <div class="col-12 _tal-l _fs-6-md _fs-7">
      <nuxt-link to="/dashboard/profile/history" class="_cl-dark">← ย้อนกลับ</nuxt-link>
    </div>
    <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-24px _pdbt-12px _fw-500 _mgbt-12px">
      รหัสงาน <span v-html="'TH0001'"></span>
      </div>
    </div>
    <div class="row _jtfct-ct _lh-175pct">
      <!-- Left Col -->
      <div class="col-md-6 col-12">
        <!-- Date and Time -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
            วัน-เวลา
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'4 กรกฎาคม 2560 / 18:00 น.'"></div>
          </div>
        </div>
        <!-- Place / Area -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
            เขต
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'ราชเทวี 10400'"></div>
          </div>
        </div>

        <!-- Shop Title -->
        <div class="row _jtfct-ct _mgt-32px">
          <div class="col-md-3 col-4 _fw-500">
            ร้านยาง
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'XXXXXX'"></div>
          </div>
        </div>
        <!-- Tire Brand -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          รายละเอียดยาง
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'xxxxxxxxx'"></div>
          </div>
        </div>
        <!-- Fee -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          ค่าตอบแทน
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'500 บาท'"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import HeaderTH from '~/components/Header'
import ActiveCard from '~/components/activeCard'
export default {
components: {
  HeaderTH,
  ActiveCard
}
}
</script>


<style lang="scss" scoped>
@import 'assets/styles/variables';
.bio-button:hover {
    background-color: $primary;
    border-width:0px ;
    transform: scale(1.05);
    transition:  0.2s;
}

</style>
