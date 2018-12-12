<template>
    <div class="container _bgcl-white box-shadow _mgbt-24px _fs-6 _bdrd-8px _lh-175pct-md _lh-150pct">
      <div class="row _jtfct-ct _pdbt-12px _pdt-16px _cl-red">
        <div class="col-12 _tal-ct _fw-500 _fs-5">
          รหัสงาน  {{ code }}
        </div>
      </div>
      <div class="row _jtfct-ct">
        <div class="col-md-3 col-4 _fw-500">
          วัน-เวลา
        </div>
        <div class="col-md-7 col-8">
          {{ datetime }}
        </div>
      </div>
      <div class="row _jtfct-ct">
        <div class="col-md-3 col-4 _fw-500">
          เขต
        </div>
        <div class="col-md-7 col-8">
          {{ place }}
        </div>
      </div>
      <div class="row _jtfct-ct">
        <div class="col-md-3 col-4 _fw-500">
          ค่าตอบแทน
        </div>
        <div class="col-md-7 col-8">
          {{ cost }} บาท
        </div>
      </div>
      <div class="row _jtfct-ct _mgbt-16px">
          <nuxt-link to="/dashboard/jobs/_slug">
            <button 
              id="show-modal" 
              class="bio-button u-rise-3-hover _mgv-16px _mgbt-24px _cl-white _bgcl-red _bdrd-4px _bdw-0px">ดูรายละเอียด
            </button>
          </nuxt-link>
      </div>
  </div>
</template>

<script>
export default {
  props: {
    code: {
      type: String,
      default: 'TH0001'
    },
    datetime: {
      type: String,
      default: '4 กรกฎาคม 2560 / 18:00 น.'
    },
    place: {
      type: String,
      default: 'ราชเทวี 10400'
    },
    cost: {
      type: String,
      default: '500'
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
