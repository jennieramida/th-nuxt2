<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container">
    <div class="row _jtfct-ct _mgt-48px">
    <div class="col-12 _tal-l-md _tal-ct _fs-6-md _fs-7">
      <nuxt-link to="/dashboard">← ย้อนกลับ</nuxt-link>
    </div>
    <div class="col-12 _cl-red _fs-4 _tal-ct _pdt-24px _pdbt-12px _fw-500 _mgbt-12px">
      รหัสงาน <span v-html="'TH0001'"></span>
      </div>
    </div>
    <div class="row _jtfct-ct _lh-175pct">
      <!-- Left Col -->
      <div class="col-md-5 col-12">
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
        <!-- Service Fee -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          ค่าตอบแทน
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'500 บาท'"></div>
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
        <!-- Shop Address -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
            ที่อยู่ร้าน
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'xxxxxxx'"></div>
          </div>
        </div>
        <!-- Shop Contact -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          ติดต่อร้าน
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'xxxxxxxxx'"></div>
          </div>
        </div>
        <!-- Customer name -->
        <div class="row _jtfct-ct _mgt-32px">
          <div class="col-md-3 col-4 _fw-500">
          ชื่อลูกค้า
          </div>
          <div class="col-md-9 col-8">
            <div v-html="'xxxxxx'"></div>
          </div>
        </div>
        <!-- Customer Address -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          ที่อยู่ลูกค้า
          </div>
          <!-- v-if can contact customer (the day of service) -->
          <!-- <div class="col-md-9 col-8">
            <div v-html="'xxxxxx'"></div>
          </div> -->
          <!-- v-if can't contact customer yet -->
          <div class="col-md-9 col-8">
            <div v-html="'ที่อยู่จะปรากฏในวันให้บริการ'"></div>
          </div>
        </div>
        <!-- Customer Contact -->
        <div class="row _jtfct-ct">
          <div class="col-md-3 col-4 _fw-500">
          ติดต่อลูกค้า
          </div>
          <!-- v-if can contact customer (the day of service) -->
          <!-- <div class="col-md-9 col-8">
            <div v-html="'xxxxxx'"></div>
          </div> -->
          <!-- v-if can't contact customer yet -->
          <div class="col-md-9 col-8">
            <div v-html="'เบอร์ติดต่อจะปรากฏในวันให้บริการ'"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row _jtfct-ct _mgt-24px">
      <nuxt-link to="/">
        <button 
          id="show-modal" 
          class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px _fs-5 _pdh-32px">รับงานนี้
        </button>
      </nuxt-link>
    </div>
  </div>
</div>
</template>

<script>
import HeaderTH from '~/components/Header'
import JobCard from '~/components/jobCard'
import ActiveCard from '~/components/activeCard'
export default {
components: {
  HeaderTH,
  JobCard,
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
