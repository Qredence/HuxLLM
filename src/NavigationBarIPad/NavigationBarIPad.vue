<script setup>
import { defineProps } from "vue";
import ControlsLeadingButtonsButtons1 from "../ControlsLeadingButtonsButtons1/ControlsLeadingButtonsButtons1.vue";
import ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly from "../ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly/ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly.vue";
import ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly from "../ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly/ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly.vue";
import ControlsTrailingButtonsButtons2 from "../ControlsTrailingButtonsButtons2/ControlsTrailingButtonsButtons2.vue";
import TwitterLogo from "../TwitterLogo/TwitterLogo.vue";
import GithubLogo from "../GithubLogo/GithubLogo.vue";

defineProps({});
</script>

<template>
  <div class="navigation-bar-i-pad">
    <div class="navigation-bar-i-pad2">
      <div class="title-and-controls">
        <div class="leading-controls">
          <ControlsLeadingButtonsButtons1
            buttons="1"
            class="leading-instance"
          ></ControlsLeadingButtonsButtons1>
          <div class="document-title">
            <div class="title">Qredence.ai</div>
            <svg
              class="down-arrow-circle"
              width="14"
              height="14"
              viewBox="0 0 14 14"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M6.84815 13.8357C7.79005 13.8357 8.67377 13.6586 9.49932 13.3044C10.3249 12.9503 11.0521 12.4564 11.6809 11.8228C12.3098 11.1891 12.8029 10.46 13.1603 9.6355C13.5176 8.81095 13.6963 7.93107 13.6963 6.99585C13.6963 6.06063 13.5176 5.18075 13.1603 4.3562C12.8029 3.53166 12.3084 2.80396 11.6768 2.1731C11.0451 1.54224 10.3166 1.04972 9.49101 0.695557C8.66546 0.34139 7.78174 0.164307 6.83984 0.164307C5.90348 0.164307 5.02253 0.34139 4.19699 0.695557C3.37144 1.04972 2.64424 1.54224 2.01538 2.1731C1.38653 2.80396 0.893418 3.53166 0.536051 4.3562C0.178684 5.18075 0 6.06063 0 6.99585C0 7.93107 0.178684 8.81095 0.536051 9.6355C0.893418 10.46 1.38791 11.1891 2.01954 11.8228C2.65117 12.4564 3.37975 12.9503 4.2053 13.3044C5.03084 13.6586 5.9118 13.8357 6.84815 13.8357Z"
                fill="#787880"
                fill-opacity="0.2"
              />
              <path
                d="M6.85254 9.51929C6.54503 9.51929 6.26662 9.38924 6.01729 9.12915L3.50741 6.4397C3.37998 6.30135 3.31488 6.13949 3.31211 5.9541C3.30934 5.76872 3.36613 5.61515 3.48248 5.49341C3.62654 5.34953 3.79275 5.27759 3.98113 5.27759C4.16951 5.27759 4.32742 5.34676 4.45485 5.48511L6.84838 8.05005L9.25022 5.48511C9.37765 5.34676 9.53556 5.27897 9.72394 5.28174C9.91232 5.28451 10.0758 5.35506 10.2143 5.49341C10.3362 5.60962 10.3957 5.7618 10.393 5.94995C10.3902 6.1381 10.3223 6.30135 10.1893 6.4397L7.68778 9.12915C7.43845 9.38924 7.16004 9.51929 6.85254 9.51929Z"
                fill="black"
                fill-opacity="0.5"
              />
            </svg>
          </div>
        </div>
        <ControlsTrailingButtonsButtons2 class="trailing-instance">
          <template #component0>
            <ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly
              class="trailing-button-1-instance"
              label="Button"
              property1="large"
              property2="ghost"
              property3="default"
              property4="icon-only"
            >
              <template #iconInstance>
                <TwitterLogo class="twitter-logo-instance"></TwitterLogo>
              </template>
            </ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly>
          </template>
          <template #component1>
            <ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly
              class="trailing-button-1-instance"
              label="Button"
              property1="large"
              property2="ghost"
              property3="default"
              property4="icon-only"
            >
              <template #iconInstance>
                <GithubLogo class="github-logo-instance"></GithubLogo>
              </template>
            </ButtonProperty1LargeProperty2GhostProperty3DefaultProperty4IconOnly>
          </template>
        </ControlsTrailingButtonsButtons2>
        <div class="frame-3">
          <div class="title2">Chat huxLLM</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.navigation-bar-i-pad,
.navigation-bar-i-pad * {
  box-sizing: border-box;
}
.navigation-bar-i-pad {
  background: #ffffff;
  display: flex;
  flex-direction: column;
  gap: 0rem;
  align-items: flex-start;
  justify-content: flex-start;
  position: relative;
}
.navigation-bar-i-pad2 {
  background: var(--container-surface-tertiary, rgba(120, 120, 128, 0.12));
  border-style: solid;
  border-color: var(--separator-separator-thin, rgba(60, 60, 67, 0.36));
  border-width: 0rem 0rem 0.020625rem 0rem;
  padding: var(--spacing-16, 1rem) var(--spacing-4, 0.25rem)
    var(--spacing-16, 1rem) var(--spacing-4, 0.25rem);
  display: flex;
  flex-direction: column;
  gap: 0.1875rem;
  align-items: center;
  justify-content: flex-start;
  flex-shrink: 0;
  width: 90rem;
  height: 5.375rem;
  position: relative;
  backdrop-filter: blur(1.5625rem);
}
.title-and-controls {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  align-self: stretch;
  flex: 1;
  position: relative;
}
.leading-controls {
  display: flex;
  flex-direction: row;
  gap: var(--spacing-8, 0.5rem);
  align-items: center;
  justify-content: flex-start;
  flex-shrink: 0;
  position: relative;
}
.leading-instance {
  flex-shrink: 0 !important;
}
.document-title {
  padding: 0.6875rem 0rem 0.6875rem var(--spacing-16, 1rem);
  display: flex;
  flex-direction: row;
  gap: var(--spacing-8, 0.5rem);
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  position: relative;
  overflow: hidden;
}
.title {
  color: var(--text-text-primary, rgba(0, 0, 0, 0.85));
  text-align: center;
  font-family: "InterDisplay-Bold", sans-serif;
  font-size: 1.25rem;
  line-height: 1.5625rem;
  font-weight: 700;
  position: relative;
}
.down-arrow-circle {
  flex-shrink: 0;
  width: 0.85625rem;
  height: 0.854375rem;
  position: relative;
  overflow: visible;
}
.trailing-instance {
  flex-shrink: 0 !important;
}
.frame-3 {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  flex-shrink: 0;
  width: 10.375rem;
  position: absolute;
  left: 39.8125rem;
  top: 0rem;
}
.title2 {
  color: var(--text-text-primary, rgba(0, 0, 0, 0.85));
  text-align: center;
  font-family: var(
    --title-title1-emphasized-font-family,
    "SfProDisplay-Bold",
    sans-serif
  );
  font-size: var(--title-title1-emphasized-font-size, 1.75rem);
  line-height: var(--title-title1-emphasized-line-height, 2.125rem);
  font-weight: var(--title-title1-emphasized-font-weight, 700);
  position: relative;
  width: 10.375rem;
  height: 3.625rem;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* nested override styles */
.twitter-logo-instance {
  flex-shrink: 0 !important;
  width: 1.5rem !important;
  height: 1.5rem !important;
}
.trailing-button-1-instance {
  padding: var(--spacing-4, 0.25rem) !important;
  gap: var(--spacing-4, 0.25rem) !important;
  flex-shrink: 0 !important;
}
.github-logo-instance {
  flex-shrink: 0 !important;
  width: 1.5rem !important;
  height: 1.5rem !important;
}
</style>
