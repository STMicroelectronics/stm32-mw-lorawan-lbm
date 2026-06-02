

# Release Notes for
# <mark>LoRaWAN Middleware</mark>
Copyright &copy; 2025 STMicroelectronics\

[![ST logo](_htmresc/st_logo_2020.png)](https://www.st.com)

# Purpose

This Middleware provides the LBM implementation of the LoRaWAN® Stack. It is based on Semtech releases


# Update History

<label for="collapse-section26" aria-hidden="true">__V1.0.0 / 19-Dec-2025__</label>
<div>

## Main Changes

- The LoRaWAN LBM stack supports the following specifications:
  - TS001-LoRaWAN® Specification L2 1.0.4
  - Regional Parameters RP02-1.0.3 plus RP02-1.0.4 for Relay feature only
  - Relay LoRaWAN® Specification TS011-1.0.1
- Starting implementation from:
  - [v4.5.0] (https://github.com/Lora-net/SWL2001/releases/tag/v4.5.0) tag for End Device and End Device with Relay feature
  - [v4.6.0] (https://github.com/Lora-net/SWL2001/releases/tag/v4.6.0-feature-relay) tag for Relay device
- Aligned [v4.8.0](https://github.com/Lora-net/SWL2001/tree/v4.8.0) tag
- Code adaptations and improvements:
  - The LoRaWAN LBM stack can be compiled to act as simple End Device, as End Device with Relay feature or a Relay device itself
  - The LoRaWAN LBM stack was modified and adapted for CubeWL package
  - Feature: Context storage in NVM enabled
  - Add: API to enable Relay feature in Relay device with Default Relay specification configuration. It is disabled by default.
  - Fix: Duty Cycle API fixed to evaluate the cumulative time-on-air
  - Fix: Struct declarations modified/changed to avoid stack overflow issues
  - Fix: MIC calculation API definition issue fixed
- Certification tests:
  - LCTT Certification tool (GUI v3.1.0, Package v3.15.0_R1)
  - Pre-certification Class A and Class C tests suites run for EU868, AS923-1, US915, AU915, IN865 Regions:
    - End Device LBM: fully PASSed
    - Relay LBM: fully PASSed
  - Pre-certification Relay test suites run for EU868, AS923-1, US915, AU915, IN865 Regions:
    - End Device Relay LBM: fully PASSed
    - Relay LBM: fully PASSed

## Known limitations:

- ABP Activation mode is not supported
- Multicast service is not fully supported
- FUOTA is not supported
- LR-FHSS is not supported
- Class B is not supported

</div>


For complete documentation on STM32WLxx,
visit: [www.st.com/stm32wl](http://www.st.com/stm32wl)

*This release note uses up to date web standards and, for this reason, should not be opened with Internet Explorer but preferably with popular browsers such as Google Chrome, Mozilla Firefox, Opera or Microsoft Edge.*
<abbr title="Based on template cx566953 version 2.0">Info</abbr>