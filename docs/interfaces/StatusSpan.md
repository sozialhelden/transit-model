[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / StatusSpan

# Interface: StatusSpan

Defined in: types.ts:200

An elevator's operational status in a specified time range.

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "status-spans".

## Properties

### closed\_by\_incoming\_status\_spans?

> `optional` **closed\_by\_incoming\_status\_spans?**: `boolean` \| `null`

Defined in: types.ts:214

If enabled, new incoming status spans that start within the time range of this status span will automatically end this status span at their start date.

***

### description?

> `optional` **description?**: `string` \| `null`

Defined in: types.ts:229

Passenger-facing status text. Filled with the operator's own text when ingested, otherwise generated from the organization's status templates on save. Editable.

***

### elevator?

> `optional` **elevator?**: ([`ElevatorId`](../type-aliases/ElevatorId.md) \| [`Elevator`](Elevator.md))[] \| `null`

Defined in: types.ts:204

Change the location to show different elevators.

***

### end\_date?

> `optional` **end\_date?**: `string` \| `null`

Defined in: types.ts:206

***

### external\_reference\_id?

> `optional` **external\_reference\_id?**: `string` \| `null`

Defined in: types.ts:222

***

### id

> **id**: `number`

Defined in: types.ts:201

***

### is\_planned?

> `optional` **is\_planned?**: `"planned"` \| `"unplanned"` \| `null`

Defined in: types.ts:208

***

### operational\_status?

> `optional` **operational\_status?**: `"out_of_service"` \| `"unknown"` \| `"operational"` \| `null`

Defined in: types.ts:207

***

### origin\_type?

> `optional` **origin\_type?**: `"operator_reported"` \| `"from_feed"` \| `"manual_entry"` \| `"sensor_detected"` \| `"user_reported"` \| `null`

Defined in: types.ts:210

***

### original\_data?

> `optional` **original\_data?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

Defined in: types.ts:225

***

### original\_elevator\_id?

> `optional` **original\_elevator\_id?**: `string` \| `null`

Defined in: types.ts:224

***

### original\_site\_id?

> `optional` **original\_site\_id?**: `string` \| `null`

Defined in: types.ts:223

***

### pinned?

> `optional` **pinned?**: `boolean` \| `null`

Defined in: types.ts:212

If enabled, this status span will be pinned and given priority over other status spans.

***

### reason\_type?

> `optional` **reason\_type?**: `"maintenance"` \| `"failure"` \| `"under_construction"` \| `"demolition"` \| `"renovation"` \| `"vandalism"` \| `"sensor_jitter"` \| `"not_monitored"` \| `null`

Defined in: types.ts:209

***

### related\_spans?

> `optional` **related\_spans?**: ([`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan`)[] \| `null`

Defined in: types.ts:218

Other status spans that are related to this one (linked manually or by feed import logic).

***

### reported\_by?

> `optional` **reported\_by?**: `string` \| `null`

Defined in: types.ts:221

***

### site?

> `optional` **site?**: ([`StopPlaceId`](../type-aliases/StopPlaceId.md) \| [`StopPlace`](StopPlace.md))[] \| `null`

Defined in: types.ts:202

***

### start\_date?

> `optional` **start\_date?**: `string` \| `null`

Defined in: types.ts:205

***

### superseded\_by?

> `optional` **superseded\_by?**: [`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan` \| `null`

Defined in: types.ts:216

The status span that superseded this one (set automatically during imports).

***

### title?

> `optional` **title?**: `string` \| `null`

Defined in: types.ts:220

Automatically generated from description and date range.
