<template>
  <div class="anchor">
    <img src="/src/assets/logo.png" class="logo" alt="">
    <div class="pc-anchor">
      <a-anchor direction="horizontal" :items="anchorList" :targetOffset="120">
      </a-anchor>
    </div>
    <div class="mobile-anchor">
      <div class="container">
        <a-button color="#fed136" size="middle" @click="changeToggle">
          <template #icon>
            <div class="icon-list">
              <span class="item-bar"></span><span class="item-bar"></span><span class="item-bar"></span>
            </div>
          </template>
        </a-button>
        <div class="anchor-list" @click="changeToggle" :style="{
        height
      }">
          <a-anchor :affix="false" :items="anchorList" :targetOffset="120"></a-anchor>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue';
const anchorList = ref([
  {
    key: 'Intro',
    href: '#Intro',
    title: 'INTRO',
  },
  {
    key: 'Schedule',
    href: '#Schedule',
    title: 'SCHEDULE',
  },
  {
    key: 'InvitedSpeakers',
    href: '#InvitedSpeakers',
    title: 'INVITED SPEAKERS',
  },
  {
    key: 'AcceptedPapers',
    href: '#AcceptedPapers',
    title: 'ACCEPTED PAPERS',
  },
  {
    key: 'CallForPapers',
    href: '#CallForPapers',
    title: 'CALL FOR PAPERS',
  },
  {
    key: 'KeyDates',
    href: '#KeyDates',
    title: 'IMPORTANT DATES',
  },
  {
    key: 'Organizers',
    href: '#Organizers',
    title: 'ORGANIZERS',
  },
  {
    key: 'Sponsors',
    href: '#Sponsors',
    title: 'SPONSORS',
  }
])
const height = computed(() => { return !toggle.value ? '0px' : "380px" })
const toggle = ref(false)
const changeToggle = () => {
  toggle.value = !toggle.value
}
</script>

<style scoped lang="less">
@media only screen and(max-width: 960px) {
  .anchor {
    height: 54px !important;
  }

  :deep(.ant-anchor) {
    display: none;
  }

  .mobile-anchor {
    display: block !important;
  }
  .logo{
    height: 41px !important;
  }
}

.mobile-anchor {
  display: none;
  width: 100%;
  height: 54px;
  padding: 0 32px;
  position: relative;

  .anchor-list {
    top: 54px;
    position: absolute;
    left: 0;
    width: 100%;
    height: 380px;
    background: #212121;
    overflow: hidden;
    transition: height 0.3s ease, opacity 0.3s ease;
  }

  :deep(.ant-anchor) {
    display: block;

    .ant-anchor-ink-visible {
      display: none !important;
    }

    .ant-anchor-link-active {
      background: #C99931 !important;
      border-radius: none !important;
      color: #FFFFFF;
    }

    .ant-anchor-link {
      letter-spacing: 0.01em;
      background: transparent;
      border-radius: 4px;
      padding: 15px;

      &+.ant-anchor-link {
        margin-left: 0;
      }

      &:hover {
        .ant-anchor-link-title {
          color: #e5ad32;
        }
      }

      .ant-anchor-link-title {
        color: #fff;
        font-family: HarmonyOS_Sans_SC_Black;
        font-size: 14px;
        color: #FFFFFF;
        font-weight: bold;
        text-transform: none;
      }
    }
  }


  :deep(.ant-btn) {
    background: #e5ad32;
    border: none;

    .icon-list {
      padding: 0 6px;
      display: flex;
      align-items: center;
      flex-direction: column;
      gap: 4px;
    }

    .item-bar {
      display: block;
      width: 100%;
      height: 2px;
      background-color: #fff;
      border-radius: 2px;
    }
  }

  .container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }
}

.anchor {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 72px;
  background: #ffffff;
  position: fixed;
  top: 0;
  z-index: 9;
    .logo {
      height: 60px;
      position: absolute;
      left: 50px;
      background-color: white;
    }

  .pc-anchor {
    :deep(.ant-anchor) {
      width: 100%;
      border-bottom: none;

      .ant-anchor-ink {
        background: transparent;
      }

      .ant-anchor-link {
        letter-spacing: 0.01em;
        border-radius: 4px;
        padding: 15px;

        &+.ant-anchor-link {
          margin-left: 14px;
        }
        &:hover {
          .ant-anchor-link-title {
            color: #e5ad32;
          }
        }
      }
      .ant-anchor-link-active {
        background: #C99931 !important;
        border-radius: none !important;
        
        .ant-anchor-link-title{
          color: #FFFFFF;
        }
      }

      .ant-anchor-ink-visible {
        background: transparent;
      }

      .ant-anchor-link-title {
        font-family: HarmonyOS_Sans_SC_Black;
        font-size: 14px;
        font-weight: bold;
        text-transform: none;
      }
    }
  }

}
</style>
