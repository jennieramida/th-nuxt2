<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container _mgt-48px">
    <div class="row _jtfct-ct">
          <div class="col-12 _tal-l _fs-6-md _fs-7">
      <nuxt-link to="/dashboard/profile" class="_cl-dark">← โปรไฟล์ของคุณ</nuxt-link>
    </div>
      <!-- Left -->
      <div class="col-12 col-md-6 _pdt-48px _pdbt-12px _lh-175pct">
        <!-- Transaction -->
        <div class="_dp-f _jtfct-spbtw _bdbtw-1px _bdcl-red">
          <div class="_cl-red _fs-4 _fw-500 _mgbt-8px _dp-ilb _tal-l">
            ยอดเงินของคุณ
          </div>
        </div>
        <!-- Total -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px _pdt-12px">
          <div class=" col-4 _fw-500">
            ยอดทั้งหมด
          </div>
          <div class=" col-8">
            <div v-html="'XXXX บาท'"></div>
          </div>
        </div>
        <!-- Can withdral -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px">
          <div class=" col-4 _fw-500">
            สามารถถอนได้
          </div>
          <div class=" col-8">
            <div v-html="'XXXX บาท'"></div>
          </div>
        </div>
        <!-- Withdral -->
            <div class="row _jtfct-ct _mgbt-16px _mgt-0px-md _mgt-24px">
            <button 
              id="show-modal" 
              class=" bio-button header-button-red  _mgv-24px-md _mgbt-0px _cl-darkred _bdrd-4px u-rise-5-hover">ถอนเงิน
            </button>
      </div>
      </div>
      <!-- Right -->
      <div class="col-12 col-md-6 _pdt-48px _pdbt-12px ">
        <div class="_dp-f _jtfct-spbtw _bdbtw-1px _bdcl-red">
          <div class="_cl-red _fs-4 _fw-500 _mgbt-8px _dp-ilb _tal-l">
        รายการเข้า-ออก
      </div>
      </div>
      <div class=" ">
        <!-- ref -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px _pdt-12px">
          <div class=" col-md-4 col-5 _fw-500">
            Ref No. 12345445
          </div>
          <div class="_cl-red col-md-8 col-7">
            <!-- Go to slug -->
            <span class="_cl-red">
              20/03/61 18:09น.
            </span>
            <span class="_cl-red">
            ถอน 1,400 บาท
            </span>
          </div>
        </div>
        <pw-modal></pw-modal>
      </div>
        </div>
    </div>
  </div>
</div>
</template>

<script>
import HeaderTH from '~/components/Header'
import JobCard from '~/components/jobCard'
import ActiveCard from '~/components/activeCard'
import pwModal from '~/components/pwModal'
export default {
components: {
  HeaderTH,
  JobCard,
  ActiveCard,
  pwModal
}
}
</script>

<style lang="scss" scoped>
$primary: #941e2e;
.header-button-red {
  background-color: $primary;
  color: white;
  border-color: $primary;
  font-size: 20px;
  padding-left: 18px;
  padding-right: 18px;
}
</style>
