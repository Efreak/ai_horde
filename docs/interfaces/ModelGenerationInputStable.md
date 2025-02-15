[@zeldafan0225/ai_horde](../README.md) / [Exports](../modules.md) / ModelGenerationInputStable

# Interface: ModelGenerationInputStable

## Table of contents

### Properties

- [cfg\_scale](ModelGenerationInputStable.md#cfg_scale)
- [clip\_skip](ModelGenerationInputStable.md#clip_skip)
- [control\_type](ModelGenerationInputStable.md#control_type)
- [denoising\_strength](ModelGenerationInputStable.md#denoising_strength)
- [facefixer\_strength](ModelGenerationInputStable.md#facefixer_strength)
- [height](ModelGenerationInputStable.md#height)
- [hires\_fix](ModelGenerationInputStable.md#hires_fix)
- [image\_is\_control](ModelGenerationInputStable.md#image_is_control)
- [karras](ModelGenerationInputStable.md#karras)
- [loras](ModelGenerationInputStable.md#loras)
- [n](ModelGenerationInputStable.md#n)
- [post\_processing](ModelGenerationInputStable.md#post_processing)
- [return\_control\_map](ModelGenerationInputStable.md#return_control_map)
- [sampler\_name](ModelGenerationInputStable.md#sampler_name)
- [seed](ModelGenerationInputStable.md#seed)
- [seed\_variation](ModelGenerationInputStable.md#seed_variation)
- [special](ModelGenerationInputStable.md#special)
- [steps](ModelGenerationInputStable.md#steps)
- [tiling](ModelGenerationInputStable.md#tiling)
- [toggles](ModelGenerationInputStable.md#toggles)
- [width](ModelGenerationInputStable.md#width)

## Properties

### cfg\_scale

• `Optional` **cfg\_scale**: `number`

its how much the AI listens to your prompt, essentially.

**`Default`**

```ts
7.5
```

**`Minimum`**

0

**`Maximum`**

100

Multiple of 0.5

#### Defined in

[index.ts:1581](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1581)

___

### clip\_skip

• `Optional` **clip\_skip**: `number`

The number of CLIP language processor layers to skip

**`Minimum`**

1

**`Maximum`**

12

#### Defined in

[index.ts:1635](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1635)

___

### control\_type

• `Optional` **control\_type**: ``"canny"`` \| ``"hed"`` \| ``"depth"`` \| ``"normal"`` \| ``"openpose"`` \| ``"seg"`` \| ``"scribble"`` \| ``"fakescribbles"`` \| ``"hough"``

#### Defined in

[index.ts:1636](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1636)

___

### denoising\_strength

• `Optional` **denoising\_strength**: `number`

The strength of denoising

**`Minimum`**

0.01

**`Maximum`**

1

Multiple of 0.01

#### Defined in

[index.ts:1589](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1589)

___

### facefixer\_strength

• `Optional` **facefixer\_strength**: `number`

**`Example`**

```ts
0.75
```

**`Minimum`**

0

**`Maximum`**

1

#### Defined in

[index.ts:1652](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1652)

___

### height

• `Optional` **height**: `number`

The height of the image to generate

**`Default`**

```ts
512
```

**`Minimum`**

64

**`Maximum`**

3072

Multiple of 64

#### Defined in

[index.ts:1600](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1600)

___

### hires\_fix

• `Optional` **hires\_fix**: `boolean`

Set to True to process the image at base resolution before upscaling and re-processing

**`Default`**

```ts
false
```

#### Defined in

[index.ts:1629](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1629)

___

### image\_is\_control

• `Optional` **image\_is\_control**: `boolean`

Set to True if the image submitted is a pre-generated control map for ControlNet use

**`Default`**

```ts
false
```

#### Defined in

[index.ts:1641](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1641)

___

### karras

• `Optional` **karras**: `boolean`

Set to True to enable karras noise scheduling tweaks

#### Defined in

[index.ts:1617](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1617)

___

### loras

• `Optional` **loras**: { `clip?`: `number` ; `inject_trigger?`: `string` ; `model?`: `number` ; `name`: `string`  }[]

#### Defined in

[index.ts:1653](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1653)

___

### n

• `Optional` **n**: `number`

The amount of images to generate

**`Minimum`**

1

**`Maximum`**

20

#### Defined in

[index.ts:1694](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1694)

___

### post\_processing

• `Optional` **post\_processing**: (``"GFPGAN"`` \| ``"RealESRGAN_x4plus"`` \| ``"RealESRGAN_x2plus"`` \| ``"RealESRGAN_x4plus_anime_6B"`` \| ``"NMKD_Siax"`` \| ``"4x_AnimeSharp"`` \| ``"strip_background"`` \| ``"CodeFormers"``)[]

The list of post-processors to apply to the image, in the order to be applied

#### Defined in

[index.ts:1619](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1619)

___

### return\_control\_map

• `Optional` **return\_control\_map**: `boolean`

Set to True if you want the ControlNet map returned instead of a generated image

**`Default`**

```ts
false
```

#### Defined in

[index.ts:1646](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1646)

___

### sampler\_name

• `Optional` **sampler\_name**: ``"k_lms"`` \| ``"k_heun"`` \| ``"k_euler"`` \| ``"k_euler_a"`` \| ``"k_dpm_2"`` \| ``"k_dpm_2_a"`` \| ``"DDIM"`` \| ``"k_dpm_fast"`` \| ``"k_dpm_adaptive"`` \| ``"k_dpmpp_2s_a"`` \| ``"k_dpmpp_2m"`` \| ``"dpmsolver"`` \| ``"k_dpmpp_sde"``

**`Default`**

```ts
k_euler
```

#### Defined in

[index.ts:1567](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1567)

___

### seed

• `Optional` **seed**: `string`

The seed to use to generete this request.

#### Defined in

[index.ts:1591](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1591)

___

### seed\_variation

• `Optional` **seed\_variation**: `number`

If passed with multiple n, the provided seed will be incremented every time by this value

**`Minimum`**

1

**`Maximum`**

1000

#### Defined in

[index.ts:1615](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1615)

___

### special

• `Optional` **special**: `Record`<`string`, `any`\>

#### Defined in

[index.ts:1682](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1682)

___

### steps

• `Optional` **steps**: `number`

**`Default`**

```ts
30
```

**`Minimum`**

1

**`Maximum`**

500

#### Defined in

[index.ts:1688](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1688)

___

### tiling

• `Optional` **tiling**: `boolean`

Set to True to create images that stitch together seamlessly

**`Default`**

```ts
false
```

#### Defined in

[index.ts:1624](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1624)

___

### toggles

• `Optional` **toggles**: `number`[]

Special Toggles used in the SD Webui. To be documented.

**`Deprecated`**

#### Defined in

[index.ts:1572](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1572)

___

### width

• `Optional` **width**: `number`

The width of the image to generate

**`Default`**

```ts
512
```

**`Minimum`**

64

**`Maximum`**

3072

Multiple of 64

#### Defined in

[index.ts:1609](https://github.com/ZeldaFan0225/ai_horde/blob/4b01aad/index.ts#L1609)
