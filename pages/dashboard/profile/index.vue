<template>
<div class="_w-100pct Prompt">
<header-t-h></header-t-h>
  <div class="container _mgt-48px">
    <div class="row _jtfct-ct">
          <div class="col-12 _tal-l _fs-6-md _fs-7">
      <nuxt-link to="/dashboard" class="_cl-dark">← ดูงานทั้งหมด</nuxt-link>
    </div>
      <!-- Left -->
      <div class="col-12 col-md-6 _pdt-48px _pdbt-12px _lh-175pct">
        <div class="_cl-red _fs-4 _fw-500 _mgbt-24px _bdbtw-1px _bdcl-red _pdbt-8px">โปรไฟล์ของคุณ</div>
        <!-- Name -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px">
          <div class=" col-4 _fw-500">
            ชื่อ-สกุล
          </div>
          <div class=" col-8">
            <div v-html="'xxxxxxxx'"></div>
          </div>
        </div>
        <!-- Phone -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px">
          <div class=" col-4 _fw-500">
            เบอร์โทรศัพท์
          </div>
          <div class=" col-8">
            <div v-html="'080-0000000'"></div>
          </div>
        </div>
        <!-- Rating -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px">
          <div class=" col-4 _fw-500">
            คะแนนของคุณ
          </div>
          <div class=" col-8">
            <div v-html="'4.XX / 5.00'"></div>
          </div>
        </div>
        <!-- Change Password -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px">
          <div class=" col-4 _fw-500">
            แก้ไขข้อมูล
          </div>
          <div class=" col-8">
            <div @click="$modal.show('changePassword')" class="_cl-red _cs-pt">
            เปลี่ยนรหัสผ่านของคุณ
            </div >
          </div>
          <div class="col-4"></div>
          <div class="col-8 _fs-6">กรุณาติดต่อเจ้าหน้าที่เพื่อแก้ไขข้อมูลอื่นๆ</div>
        </div>
        <!-- Transaction -->
        <div class="_dp-f _jtfct-spbtw _mgt-48px _bdbtw-1px _bdcl-red">
          <div class="_cl-red _fs-4 _fw-500 _mgbt-8px _dp-ilb _tal-l">
            ยอดเงิน
          </div>
          <div class="_cl-red _fs-5-md _fs-6 _tal-r _dp-ilb">
            <nuxt-link  to="/dashboard/profile/transaction">
              <span class="_cl-red">
                ดูรายละเอียด
              </span>
            </nuxt-link>
          </div>
        </div>
        <!-- Total -->
        <div class="row _fs-5-md _fs-6 _mgv-8px-md _mgv-4px _pdt-12px">
          <div class=" col-4 _fw-500">
            ยอดเงินทั้งหมด
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
      </div>
      <!-- Right -->
      <div class="col-12 col-md-6 _pdt-48px _pdbt-12px ">
        <div class="_dp-f _jtfct-spbtw _bdbtw-1px _bdcl-red">
          <div class="_cl-red _fs-4 _fw-500 _mgbt-8px _dp-ilb _tal-l">
        ประวัติงานที่เคยรับ
      </div>
      <div class="_cl-red _fs-5-md _fs-6 _tal-r _dp-ilb">
        <nuxt-link  to="/dashboard/profile/history">
          <span class="_cl-red">
          ดูทั้งหมด
          </span>
        </nuxt-link>
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

<style>

</style>
