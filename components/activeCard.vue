<template>
    <div class="container _bgcl-white box-shadow _pst-rlt _mgbt-24px _fs-6 _bdrd-8px _lh-175pct-md _lh-150pct">
      <!-- Step 1 : Order Details -->
      <!-- <div>
        <div class="row _jtfct-ct _pdv-24px _cl-red">
          <div class="col-12 _tal-ct _fw-500 _fs-5">
            รหัสงาน  {{ code }} 
          </div> 
          <div class="col-12 _cl-positive _tal-ct">
            งานของคุณ
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-4 _fw-500">
            วัน-เวลา
          </div>
          <div class="_pdh-0px col-md-8 col-8">
            {{ datetime }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-4 _fw-500">
            เขต
          </div>
          <div class="_pdh-0px col-md-8 col-8">
            {{ place }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-4 _fw-500">
            รายละเอียดยาง
          </div>
          <div class="_pdh-0px col-md-8 col-8">
            {{ tireDetails }}
          </div>
        </div>
          <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-4 _fw-500">
            ราคายาง
          </div>
          <div class="_pdh-0px col-md-8 col-8">
            {{ tireCost }} บาท
          </div>
        </div>
      </div> -->
      <!-- Step 2 : Shop Details -->
      <!-- <div>
        <div class="row _jtfct-ct _pdv-24px _cl-red">
          <div class="col-12 _tal-ct _fw-500 _fs-5">
            รหัสงาน  {{ code }} 
          </div> 
          <div class="col-12 _cl-positive _tal-ct">
            กำลังดำเนินการ (ไปรับยาง)
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            ร้านยาง
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ shopName }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            เบอร์ติดต่อร้าน
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ phone }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            รายละเอียดยาง
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ tireDetails }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            ราคายาง
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ tireCost }} บาท
          </div>
        </div>
          <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            ที่อยู่ร้าน
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            <a href="/" target="_blank">link to google map</a>
          </div>
        </div>
      </div> -->
      <!-- Step 3 : Customer -->
      <div>
        <div class="row _jtfct-ct _pdv-24px _cl-red">
          <div class="col-12 _tal-ct _fw-500 _fs-5">
            รหัสงาน  {{ code }} 
          </div> 
          <div class="col-12 _cl-positive _tal-ct">
            กำลังดำเนินการ
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            ชื่อลูกค้า
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ customerName }}
          </div>
        </div>
        <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            เบอร์ติดต่อ
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            {{ phone }}
          </div>
        </div>
          <div class="row _jtfct-ct">
          <div class="_pdl-0px _tal-r col-md-4 col-5 _fw-500">
            ที่อยู่ลูกค้า
          </div>
          <div class="_pdh-0px col-md-8 col-7">
            <a href="/" target="_blank">link to google map</a>
          </div>
        </div>
      </div>
      <!-- button -->
      <div class="row _jtfct-ct _mgbt-16px">
          <nuxt-link to="/dashboard/jobs/active/_slug">
            <button 
              id="show-modal" 
              class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">ดำเนินการ
            </button>
          </nuxt-link>
      </div>
      <!-- Disable -->
      <!-- <button class="bio-button -disabled u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">ดำเนินการ
      </button> -->
      <!-- done -->
      <!-- <div class="row _jtfct-ct _mgbt-16px">
        <button 
          class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">เสร็จสิ้นการดำเนินการ
        </button>
      </div> -->
  </div>
</template>

<script>
export default {
  props: {
    code: {
      type: String,
      default: 'TH0001'
    },
    customerName: {
      type: String,
      default: 'xxxxx'
    },
    phone: {
      type: String,
      default: 'xxxxx'
    },
    tireDetails: {
      type: String,
      default: '160/45/17 Michelin 4 ชิ้น'
    },
    tireCost: {
      type: String,
      default: 'xxxx'
    }
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
