<template>
  <header>
    <div class="container-fluid Prompt _bgcl-red"> 
    <div class="container">
        <div class="row _pdv-16px _alit-ct _jtfct-spbtw">
        <div class="col-md-2 col-6">
          <nuxt-link to="/dashboard">
            <img src="~/assets/images/logo.svg" class="_h-48px-md _h-32px">
          </nuxt-link>
        </div>
        <div class="col-md-10 _dp-f-md _dp-n _jtfct-fe _pdl-128px _alit-ct">
           <div class="_mgr-24px">
            <nuxt-link 
              to="/dashboard"> 
              <span 
                class="hover-underline-animation _cl-white"> งานทั้งหมด</span>
            </nuxt-link>
          </div>
          <div class="_mgr-24px">
            <nuxt-link 
              to="/dashboard/profile"> 
              <span 
                class="hover-underline-animation _cl-white"> โปรไฟล์ของคุณ</span>
            </nuxt-link>
          </div>
          <div class="_mgr-24px">
            <nuxt-link 
              to="/dashboard/profile/history"> 
              <span
                class="hover-underline-animation _cl-white">ประวัติงานทั้งหมด</span>
            </nuxt-link>
          </div>
          <div>
            <nuxt-link 
              to="/signin"
              class="hover-underline-animation _cl-white">
              ออกจากระบบ
            </nuxt-link>
          </div>
        </div>
        <div class="col-6 _dp-f _dp-n-md _jtfct-fe">
          <button
            :class="{'-open': isShowingMenu }"
            class="bio-button _pd-0px _zid-1 _bgcl-tpr _bdcl-tpr hamburger-container _w-32px _h-32px _dp-f"
            @click=" isShowingMenu = !isShowingMenu">
            <div class="hamburger-btn"/>
          </button>
          <fade-transition>
            <HBGMenu v-show="isShowingMenu"/>
          </fade-transition>
        </div>
      </div>
    </div>
    </div>
  </header>
</template>

<script>
import HBGMenu from '~/components/HBGMenu'
export default {
  components: {
    HBGMenu
  },
  data:() => ({
    isShowingMenu: false
  })
}
</script>

<style lang="scss" scoped>
$primary: #941e2e;

.header-mobile {
  background-color: white;
  box-shadow: 0px 0px 5px 1px gainsboro;
}
._cl-darkred {
  color: $primary;
}
.header-button {
  background-color: transparent;
  border-color: $primary;
  &:hover {
    background-color: $primary;
    color: white;
    transition: 0.3s;
  }
}

:any-link {
  color: rgba(0, 0, 0, 0.7);
}

.hover-underline-animation {
  display: inline-block;
  position: relative;
  cursor: pointer;
  &::after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0) translateY(4px);
    height: 1px;
    bottom: 0;
    left: 0;
    background-color: white;
    transform-origin: bottom right;
    transition: transform 0.25s ease-out;
    cursor: pointer;
  }
}

.hover-underline-animation:hover::after {
  transform: scaleX(1) translateY(4px);
  transform-origin: bottom left;
  cursor: pointer;
}

.hamburger-btn {
  width: 33px;
  height: 3px;
  background: white;
  border-radius: 8px;
  position: absolute;
  transition: 0.2s;
  :not(.-open) {
    &:hover {
      width: 28px;
      &::before {
        width: 33px;
      }
      &::after {
        width: 30px;
      }
    }
  }

  &::before {
    width: 28px;
    position: absolute;
    height: 3px;
    background: white;
    border-radius: 8px;
    content: ' ';
    top: -11px;
    right: 0px;
    transition: 0.2s;
  }

  &::after {
    position: absolute;
    width: 28px;
    height: 3px;
    background: white;
    border-radius: 8px;
    content: ' ';
    top: 11px;
    right: 0px;
    transition: 0.2s;
  }
}

.hamburger-container {
  z-index: 70 !important;
  &.-open {
    .hamburger-btn {
      background: $primary;
      background-color: $primary;
      position: fixed;
      &::before {
        width: 33px;
        top: 0px;
        transform: rotate(-45deg);
        transition: 0.2s;
        background: white;
        content: ' ';
        &:hover {
          width: 33px;
        }
      }
      &::after {
        width: 33px;
        top: 0px;
        transform: rotate(45deg);
        transition: 0.2s;
        background: white;
        content: ' ';
        &:hover {
          width: 33px;
        }
      }
    }
  }
}
</style>
