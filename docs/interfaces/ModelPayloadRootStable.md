[@zeldafan0225/stable_horde](../README.md) / [Exports](../modules.md) / ModelPayloadRootStable

# Interface: ModelPayloadRootStable

## Table of contents

### Properties

- [cfg\_scale](ModelPayloadRootStable.md#cfg_scale)
- [denoising\_strength](ModelPayloadRootStable.md#denoising_strength)
- [height](ModelPayloadRootStable.md#height)
- [karras](ModelPayloadRootStable.md#karras)
- [sampler\_name](ModelPayloadRootStable.md#sampler_name)
- [seed](ModelPayloadRootStable.md#seed)
- [seed\_variation](ModelPayloadRootStable.md#seed_variation)
- [toggles](ModelPayloadRootStable.md#toggles)
- [use\_gfpgan](ModelPayloadRootStable.md#use_gfpgan)
- [use\_ldsr](ModelPayloadRootStable.md#use_ldsr)
- [use\_real\_esrgan](ModelPayloadRootStable.md#use_real_esrgan)
- [use\_upscaling](ModelPayloadRootStable.md#use_upscaling)
- [width](ModelPayloadRootStable.md#width)

## Properties

### cfg\_scale

• `Optional` **cfg\_scale**: `number`

its how much the AI listens to your prompt, essentially.

**`Default`**

5

**`Minimum`**

-40

**`Maximum`**

30

Multiple of 0.5

#### Defined in

[index.ts:1631](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1631)

___

### denoising\_strength

• `Optional` **denoising\_strength**: `number`

The strength of denoising

**`Minimum`**

0

**`Maximum`**

1

Multiple of 0.01

#### Defined in

[index.ts:1639](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1639)

___

### height

• `Optional` **height**: `number`

The height of the image to generate

**`Default`**

512

**`Minimum`**

64

**`Maximum`**

1024

Multiple of 64

#### Defined in

[index.ts:1650](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1650)

___

### karras

• `Optional` **karras**: `boolean`

Set to True to enable karras noise scheduling tweaks

#### Defined in

[index.ts:1667](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1667)

___

### sampler\_name

• `Optional` **sampler\_name**: `k_lms` \| `k_heun` \| `k_euler` \| `k_dpm_2` \| `k_dpm_2_a` \| `DDIM` \| `PLMS` \| `k_dpm_fast` \| `k_dpm_adaptive` \| `k_dpmpp_2s_a` \| `k_dpmpp_2m` \| `dpmsolver`

**`Default`**

k_euler

#### Defined in

[index.ts:1618](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1618)

___

### seed

• `Optional` **seed**: `string`

The seed to use to generete this request.

#### Defined in

[index.ts:1641](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1641)

___

### seed\_variation

• `Optional` **seed\_variation**: `number`

If passed with multiple n, the provided seed will be incremented every time by this value

**`Minimum`**

1

**`Maximum`**

1000

#### Defined in

[index.ts:1665](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1665)

___

### toggles

• `Optional` **toggles**: `number`[]

Special Toggles used in the SD Webui. To be documented.

#### Defined in

[index.ts:1622](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1622)

___

### use\_gfpgan

• `Optional` **use\_gfpgan**: `boolean`

Set to true to process the generated image with GFPGAN (face correction)

#### Defined in

[index.ts:1669](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1669)

___

### use\_ldsr

• `Optional` **use\_ldsr**: `boolean`

Set to true to process the generated image with LDSR

#### Defined in

[index.ts:1673](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1673)

___

### use\_real\_esrgan

• `Optional` **use\_real\_esrgan**: `boolean`

Set to true to process the generated image with RealESRGAN

#### Defined in

[index.ts:1671](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1671)

___

### use\_upscaling

• `Optional` **use\_upscaling**: `boolean`

Set to true to upscale the image

#### Defined in

[index.ts:1675](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1675)

___

### width

• `Optional` **width**: `number`

The width of the image to generate

**`Default`**

512

**`Minimum`**

64

**`Maximum`**

1024

Multiple of 64

#### Defined in

[index.ts:1659](https://github.com/ZeldaFan0225/stable_horde/blob/cc34adc/index.ts#L1659)