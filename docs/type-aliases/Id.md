[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / Id

# Type Alias: Id\<Brand\>

> **Id**\<`Brand`\> = `number` & `object`

Defined in: [types.ts:15](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L15)

A branded numeric ID. Assignable to `number`, but tagged with its collection so that
e.g. a StopPlaceId cannot be passed where a SchemaOrganizationId is expected.
Brand a raw number with [asId](../functions/asId.md).

## Type Declaration

### \_\_idBrand

> `readonly` **\_\_idBrand**: `Brand`

## Type Parameters

### Brand

`Brand` *extends* `string`
