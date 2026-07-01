[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / StopPlace

# Interface: StopPlace

Defined in: types.ts:138

A transit-relevant site, station, stop area, or stop place.

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "stop-places".

## Properties

### generateSlug?

> `optional` **generateSlug?**: `boolean` \| `null`

Defined in: types.ts:169

When enabled, the slug will auto-generate from the title field on save and autosave.

***

### holiday\_region?

> `optional` **holiday\_region?**: `object`

Defined in: types.ts:176

Determines which public holidays apply. Uses the elevator/site location to select regional holidays.

#### country\_code?

> `optional` **country\_code?**: `string` \| `null`

ISO 3166-1 alpha-2 country code (e.g. "de", "at", "ch")

#### current\_holiday?

> `optional` **current\_holiday?**: `string` \| `null`

Shows the name of today's public holiday (if any) for the configured region.

#### state?

> `optional` **state?**: `string` \| `null`

State or region name for regional holidays (e.g. "Berlin", "Bayern", "Wien")

#### upcoming\_holidays?

> `optional` **upcoming\_holidays?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

Next public holidays for the configured region (90 days ahead).

***

### id

> **id**: `number`

Defined in: types.ts:139

***

### internal\_description?

> `optional` **internal\_description?**: `string` \| `null`

Defined in: types.ts:142

***

### linked\_data?

> `optional` **linked\_data?**: `object`

Defined in: types.ts:144

#### maintenance\_org?

> `optional` **maintenance\_org?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md) \| `null`

#### owner\_org?

> `optional` **owner\_org?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md) \| `null`

#### transit\_networks\_served?

> `optional` **transit\_networks\_served?**: ([`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md))[] \| `null`

#### url?

> `optional` **url?**: `object`[] \| `null`

***

### main\_identifier?

> `optional` **main\_identifier?**: `string` \| `null`

Defined in: types.ts:143

***

### modes?

> `optional` **modes?**: `object`

Defined in: types.ts:188

#### servicedTransportModes?

> `optional` **servicedTransportModes?**: [`TransitModeId`](../type-aliases/TransitModeId.md)[] \| `null`

Means of transport serviced at this stop place.

***

### normalized\_name?

> `optional` **normalized\_name?**: `string` \| `null`

Defined in: types.ts:141

The normalized name of the site, used for display and search purposes.

***

### normalized\_names?

> `optional` **normalized\_names?**: `object`

Defined in: types.ts:155

Preprocessed station names to improve searchability and sorting.

#### clean\_name\_db?

> `optional` **clean\_name\_db?**: `string` \| `null`

#### clean\_name\_vbb?

> `optional` **clean\_name\_vbb?**: `string` \| `null`

#### normalization\_warnings?

> `optional` **normalization\_warnings?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

#### tokenized\_name\_db?

> `optional` **tokenized\_name\_db?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

#### tokenized\_name\_vbb?

> `optional` **tokenized\_name\_vbb?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

***

### now\_open?

> `optional` **now\_open?**: `boolean` \| `null`

Defined in: types.ts:174

Automatically calculated based on opening hours, current time, and regional public holidays.

***

### opening\_hours?

> `optional` **opening\_hours?**: `string` \| `null`

Defined in: types.ts:172

Example: "Mo-Fr 06:00-22:00; Sa-Su 08:00-20:00; PH off". OSM-compatible format. Use "PH off" to close on public holidays. https://openingh.openstreetmap.de/evaluation_tool/

***

### slug

> **slug**: `string`

Defined in: types.ts:170
