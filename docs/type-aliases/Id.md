[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / Id

# Type Alias: Id\<Brand\>

> **Id**\<`Brand`\> = `number` & `object`

Defined in: types.ts:15

A branded numeric ID. Assignable to `number`, but tagged with its collection so that
e.g. a StopPlaceId cannot be passed where a SchemaOrganizationId is expected.
Brand a raw number with [asId](../functions/asId.md).

## Type Declaration

### \_\_idBrand

> `readonly` **\_\_idBrand**: `Brand`

## Type Parameters

### Brand

`Brand` *extends* `string`
