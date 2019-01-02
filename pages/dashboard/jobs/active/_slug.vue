<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container _fs-7 _fs-6-md">
    <div class="row _jtfct-ct _mgt-48px-md _mgt-12px">
    <div class="col-12 _cl-red _fs-5 _tal-l-md _tal-ct _pdt-24px _pdbt-12px _fw-500">
      รหัสงาน <span v-html="'TH0001'"></span>
    </div>
    </div>
    <div class="row _jtfct-ct _lh-175pct">
      <!-- Left Col -->
      <div class="col-12">
        <!-- Date and Time -->
        <div class="row ">
          <div class="col-md-2  _tal-l-md col-4 _fw-500">
            วัน-เวลา
          </div>
          <div class="col-md-4 col-8">
            <div v-html="'4 กรกฎาคม 2560 / 18:00 น.'"></div>
          </div>
        </div>
        <!-- Place / Area -->
        <div class="row ">
          <div class="col-md-2  _tal-l-md col-4 _fw-500">
            เขต
          </div>
          <div class="col-md-4 col-8">
            <div v-html="'ราชเทวี 10400'"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="row _mgv-24px">
      <div class="col-12 _cl-red _fs-5 _tal-l-md _tal-ct  _pdbt-12px _pdbt-24px-md _fw-500">
      สถานะการดำเนินการ
      </div>
      <!-- _cl-red if active -->
      <div class="col-4 _pdv-8px _cs-pt _tal-ct _bdtw-1px _bdbtw-1px _bdrw-1px _bdcl-red _cl-white _bgcl-red">
      รายละเอียดงาน
      </div>
      <div class="col-4 _pdv-8px _cs-pt _tal-ct _bdtw-1px _bdbtw-1px _bdrw-1px _bdcl-red _cl-red">
      รับยางจากร้าน 
      </div>
      <div class="col-4 _pdv-8px _cs-pt _tal-ct _bdtw-1px _bdbtw-1px _bdcl-red _cl-red">
      เปลี่ยนยาง
      </div>
    </div>
    <!-- Order Details -->
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        รายละเอียดยาง
      </div>
      <div class="col-md-4 col-8">
        <div v-html="'160/45/17 Michelin 4 ชิ้น'"></div>
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        ราคายาง
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'xxxx'"></span> บาท
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        หมายเหตุ
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'xxxxxxxxxx'"></span>
      </div>
    </div>

    <!-- Shop Details -->
    <!-- <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        ชื่อร้านยาง
      </div>
      <div class="col-md-4 col-8">
        <div v-html="'xxxxx'"></div>
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        เบอร์ติดต่อร้าน
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'0989393939'"></span>
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        ที่อยู่ร้าน
      </div>
      <div class="col-md-4 col-8">
        <a href="" target="_blank" class="_cl-red">link to google map</a>
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        หมายเหตุ
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'xxxxxxxxxx'"></span>
      </div>
    </div>
    <div class="row _mgt-24px _jtfct-ct">
      <div class="col-11 _bgcl-accent _pdt-64px _pdbt-128px">map</div>
    </div> -->

    <!-- customer Details -->
    <!-- <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        ชื่อลูกค้า
      </div>
      <div class="col-md-4 col-8">
        <div v-html="'xxxxx'"></div>
      </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        เบอร์ติดต่อ
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'0989393939'"></span>
      </div>
    </div>
    <div class="row _mgt-4px">
        <div class="col-md-2  _tal-l-md col-4 _fw-500">
          ที่อยู่ร้าน
        </div>
        <div class="col-md-4 col-8">
          <a href="" target="_blank" class="_cl-red">link to google map</a>
        </div>
    </div>
    <div class="row _mgt-4px">
      <div class="col-md-2  _tal-l-md col-4 _fw-500">
        หมายเหตุ
      </div>
      <div class="col-md-4 col-8">
        <span v-html="'xxxxxxxxxx'"></span>
      </div>
    </div>
    <div class="row _mgt-24px _jtfct-ct">
      <div class="col-11 _bgcl-accent _pdt-64px _pdbt-128px">map</div>
    </div> -->

    <!-- Button -->
    <div class="row _jtfct-ct _mgv-16px">
      <!-- Can click -->
      <button 
        class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">ดำเนินการ
      </button>
      <!-- Disable -->
      <!-- <button class="bio-button -disabled u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">ดำเนินการ
      </button> -->
      <!-- Done -->
      <!-- <button 
        class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">เสร็จสิ้นการดำเนินการ
      </button> -->
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
