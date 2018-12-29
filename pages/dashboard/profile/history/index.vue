<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container _mgt-48px">
    <div class="row _jtfct-ct">
          <div class="col-12 _tal-l _fs-6-md _fs-7">
      <nuxt-link to="/dashboard/profile" class="_cl-dark">← โปรไฟล์ของคุณ</nuxt-link>
    </div>
      <!-- Right -->
      <div class="col-12 _pdt-48px _pdbt-12px ">
        <div class="_dp-f _jtfct-spbtw _bdbtw-1px _bdcl-red">
          <div class="_cl-red _fs-4 _fw-500 _mgbt-8px _dp-ilb _tal-l">
        ประวัติงานที่เคยรับ
      </div>
      </div>
      <div class=" ">
        <!-- Name -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px _pdt-12px">
          <div class=" col-md-4 col-5 _fw-500">
            รหัสงาน TH0001
          </div>
          <div class="_cl-red col-md-8 col-7">
            <!-- Go to slug -->
            <nuxt-link  to="/dashboard/profile/history/_slug">
            <span class="_cl-red">
            ดูรายละเอียด
            </span>
            </nuxt-link>
          </div>
        </div>
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
export default {
components: {
  HeaderTH,
  JobCard,
  ActiveCard
}
}
</script>

<style>

</style>
