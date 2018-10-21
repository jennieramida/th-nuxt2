<template>
<div class="_w-100pct _bgcl-red Prompt _h-100vh _dp-f _alit-ct">
  <div class="container">
    <div class="row _mgh-0px _w-100pct _jtfct-ct">
      <div class="col-12 _dp-f _jtfct-ct">
          <img src="~/assets/images/logo.svg" alt="">
      </div>
      <div class="col-12 _cl-white _dp-f _jtfct-ct _fs-4 _fw-500 _mgt-48px">
        เข้าสู่ระบบช่าง
      </div>
    </div>
    <div class="row _mgh-0px _dp-f _jtfct-ct _w-100pct">
      <div class="col-12 col-md-4 _pdbt-48px _pdbt-0px-md _cl-white">
        <div class="_pdt-24px _pdbt-4px">อีเมล</div>
        <div class="bio-input">
          <input 
            type="email" 
            placeholder="โปรดกรอกอีเมล">
        </div>
        <div class="_pdt-24px _pdbt-4px">รหัสผ่าน</div>
        <div class="bio-input">
          <input 
            type="password"
            placeholder="โปรดตั้งรหัสผ่านใหม่">
        </div>
        <div 
          v-scroll-reveal="{viewFactor:0.5, delay:100,scale: 1, origin:'top', distance:'20px', easing: 'cubic-bezier(0.6, 0.2, 0.1, 1)' , opacity: 0, duration: 1000}" 
          class="_dp-f _jtfct-ct _pdv-24px _pdt-48px _pdt-24px-md ">
          <button 
            id="show-modal" 
            class="bio-button header-button u-rise-5-hover _mgv-24px-md _mgbt-0px _cl-darkred _bdrd-4px u-rise-5-hover">เข้าสู่ระบบ
          </button>
        </div>
        <div class="_fs-6 _mgt-12px _pdt-12px _tal-ct">
          สมัครเป็นช่างกับ Tireshouse 
          <span
            to="/signin"
            class="_cl-darkred _cs-pt _bdbtw-1px" 
            @click="$modal.show('login')">
            กดที่นี่</span>
        </div>
      </div>
    </div>
  </div>
</div>
</template>


<style lang="scss" scoped>
@import 'assets/styles/variables';
.header-button {
  background-color: white;
  color: $primary;
  border-color: white;
  font-size: 20px;
  padding-left: 18px;
  padding-right: 18px;
}

input::placeholder {
  font-family: Prompt !important;
  font-weight: 300 !important;
}
</style>
