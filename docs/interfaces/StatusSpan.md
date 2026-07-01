[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / StatusSpan

# Interface: StatusSpan

Defined in: [types.ts:200](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L200)

An elevator's operational status in a specified time range.

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "status-spans".

## Properties

### closed\_by\_incoming\_status\_spans?

> `optional` **closed\_by\_incoming\_status\_spans?**: `boolean` \| `null`

Defined in: [types.ts:214](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L214)

If enabled, new incoming status spans that start within the time range of this status span will automatically end this status span at their start date.

***

### description?

> `optional` **description?**: `string` \| `null`

Defined in: [types.ts:229](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L229)

Passenger-facing status text. Filled with the operator's own text when ingested, otherwise generated from the organization's status templates on save. Editable.

***

### elevator?

> `optional` **elevator?**: ([`ElevatorId`](../type-aliases/ElevatorId.md) \| [`Elevator`](Elevator.md))[] \| `null`

Defined in: [types.ts:204](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L204)

Change the location to show different elevators.

***

### end\_date?

> `optional` **end\_date?**: `string` \| `null`

Defined in: [types.ts:206](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L206)

***

### external\_reference\_id?

> `optional` **external\_reference\_id?**: `string` \| `null`

Defined in: [types.ts:222](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L222)

***

### id

> **id**: `number`

Defined in: [types.ts:201](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L201)

***

### is\_planned?

> `optional` **is\_planned?**: `"planned"` \| `"unplanned"` \| `null`

Defined in: [types.ts:208](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L208)

***

### operational\_status?

> `optional` **operational\_status?**: `"out_of_service"` \| `"unknown"` \| `"operational"` \| `null`

Defined in: [types.ts:207](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L207)

***

### origin\_type?

> `optional` **origin\_type?**: `"operator_reported"` \| `"from_feed"` \| `"manual_entry"` \| `"sensor_detected"` \| `"user_reported"` \| `null`

Defined in: [types.ts:210](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L210)

***

### original\_data?

> `optional` **original\_data?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

Defined in: [types.ts:225](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L225)

***

### original\_elevator\_id?

> `optional` **original\_elevator\_id?**: `string` \| `null`

Defined in: [types.ts:224](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L224)

***

### original\_site\_id?

> `optional` **original\_site\_id?**: `string` \| `null`

Defined in: [types.ts:223](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L223)

***

### pinned?

> `optional` **pinned?**: `boolean` \| `null`

Defined in: [types.ts:212](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L212)

If enabled, this status span will be pinned and given priority over other status spans.

***

### reason\_type?

> `optional` **reason\_type?**: `"maintenance"` \| `"failure"` \| `"under_construction"` \| `"demolition"` \| `"renovation"` \| `"vandalism"` \| `"sensor_jitter"` \| `"not_monitored"` \| `null`

Defined in: [types.ts:209](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L209)

***

### related\_spans?

> `optional` **related\_spans?**: ([`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan`)[] \| `null`

Defined in: [types.ts:218](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L218)

Other status spans that are related to this one (linked manually or by feed import logic).

***

### reported\_by?

> `optional` **reported\_by?**: `string` \| `null`

Defined in: [types.ts:221](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L221)

***

### site?

> `optional` **site?**: ([`StopPlaceId`](../type-aliases/StopPlaceId.md) \| [`StopPlace`](StopPlace.md))[] \| `null`

Defined in: [types.ts:202](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L202)

***

### start\_date?

> `optional` **start\_date?**: `string` \| `null`

Defined in: [types.ts:205](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L205)

***

### superseded\_by?

> `optional` **superseded\_by?**: [`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan` \| `null`

Defined in: [types.ts:216](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L216)

The status span that superseded this one (set automatically during imports).

***

### title?

> `optional` **title?**: `string` \| `null`

Defined in: [types.ts:220](https://github.com/sozialhelden/transit-model/blob/d56e91565a6bacd9bd7a5d499c4e4b62f67a6c5d/src/types.ts#L220)

Automatically generated from description and date range.
