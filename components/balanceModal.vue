<template>
  <modal 
    name="balance" 
    height="auto">
    <div class="container modal-size _dp-f _alit-ct _jtfct-ct _fdrt-cl _pdbt-24px _mg-0px">
      <div class="row _w-100pct _alit-ct _dp-f _jtfct-ct">
        <div class="col _pdh-12px">
          <div class="_fs-3 _cl-black _tal-ct _pdt-64px">ถอนเงิน</div>
          <div class="_pdt-24px _fs-5 _cl-black _pdbt-8px">จำนวนเงินที่ต้องการถอน</div>
          <div class="bio-input">
            <input 
              type="text" 
              placeholder="ระบุจำนวนเงินที่ต้องการถอน">
          </div>
          <div class="_fs-7 _mgt-12px">ยอดเงินที่ถอนได้: <span v-html="'1,500 บาท'" class="_cl-red"/></div>
          <div class="_fs-7 _mgt-4px">ค่าธรรมเนียม: <span v-html="'20 บาท'" class="_cl-red"/> ต่อครั้ง</div>
          <div class="_dp-f _jtfct-spbtw _mgt-24px">
            <button  @click="$modal.hide('balance')" class="bio-button -dark _opct-40 _mgv-24px-md _mgbt-0px _cl-white _bdrd-4px">
                ยกเลิก
            </button>
            <button class="bio-button header-button-red _mgv-24px-md _mgbt-0px _cl-darkred _bdrd-4px u-rise-5-hover">
                ยืนยันการทำรายการ
            </button>
          </div>
    
      
        </div>
      </div>
    </div>
  </modal>
</template>



<style lang="scss" scoped>
@import 'assets/styles/variables';
.modal-size {
  min-height: 50vh;
  max-width: 50vw;
 @media (max-width: $md - 1px) {
   max-width: 100vw;
 }
}

$primary: #941e2e;
$secondary: #f8f8f9;

._cl-darkred {
  color: $primary;
}

.header-button-red {
  background-color: $primary;
  color: white;
  border-color: $primary;
  font-size: 20px;
  padding-left: 18px;
  padding-right: 18px;
}

input::placeholder {
  font-family: 'Prompt' !important;
}
</style>
