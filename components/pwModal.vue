<template>
  <modal 
    name="changePassword" 
    height="auto">
    <div class="container modal-size _dp-f _alit-ct _fdrt-cl _pdbt-24px">
      <div class="row _w-100pct">
        <div class="col _pdh-12px">
          <div class="_fs-2 _cl-black _tal-ct _pdt-64px">เปลี่ยนรหัสผ่าน</div>
          <div class="_pdt-24px _fs-5 _cl-black _pdbt-8px">รหัสผ่านเดิม</div>
          <div class="bio-input">
            <input 
              type="password" 
              placeholder="โปรดกรอกรหัสผ่านใหม่">
          </div>
          <div class="_pdt-24px _fs-5 _cl-black _pdbt-8px">รหัสผ่านใหม่</div>
          <div class="bio-input">
            <input 
              type="password"
              placeholder="โปรดกรอกรหัสผ่านใหม่">
          </div>
          <div class="_pdt-24px _fs-5 _cl-black _pdbt-8px">ยืนยันรหัสผ่าน</div>
          <div class="bio-input">
            <input 
              type="password"
              placeholder="โปรดยืนยันรหัสผ่าน">
          </div>
          <div class="_dp-f _jtfct-spbtw _mgt-24px">
            <button  @click="$modal.hide('changePassword')" class="bio-button -dark _opct-40 _mgv-24px-md _mgbt-0px _cl-white _bdrd-4px">
                ยกเลิก
            </button>
            <button class="bio-button header-button-red _mgv-24px-md _mgbt-0px _cl-darkred _bdrd-4px u-rise-5-hover">
                เปลี่ยนรหัสผ่าน
            </button>
          </div>
    
      
        </div>
      </div>
    </div>
  </modal>
</template>



<style lang="scss" scoped>
.modal-size {
  min-height: 70vh;
  max-width: 50vw;
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
