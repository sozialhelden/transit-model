[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / StatusSpan

# Interface: StatusSpan

Defined in: [types.ts:223](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L223)

An elevator's operational status in a specified time range.

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "status-spans".

## Properties

### closed\_by\_incoming\_status\_spans?

> `optional` **closed\_by\_incoming\_status\_spans?**: `boolean` \| `null`

Defined in: [types.ts:237](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L237)

If enabled, new incoming status spans that start within the time range of this status span will automatically end this status span at their start date.

***

### description?

> `optional` **description?**: `string` \| `null`

Defined in: [types.ts:252](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L252)

Passenger-facing status text. Filled with the operator's own text when ingested, otherwise generated from the organization's status templates on save. Editable.

***

### elevator?

> `optional` **elevator?**: ([`ElevatorId`](../type-aliases/ElevatorId.md) \| [`Elevator`](Elevator.md))[] \| `null`

Defined in: [types.ts:227](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L227)

Change the location to show different elevators.

***

### end\_date?

> `optional` **end\_date?**: `string` \| `null`

Defined in: [types.ts:229](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L229)

***

### external\_reference\_id?

> `optional` **external\_reference\_id?**: `string` \| `null`

Defined in: [types.ts:245](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L245)

***

### id

> **id**: `number`

Defined in: [types.ts:224](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L224)

***

### is\_planned?

> `optional` **is\_planned?**: `"planned"` \| `"unplanned"` \| `null`

Defined in: [types.ts:231](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L231)

***

### location?

> `optional` **location?**: `object`

Defined in: [types.ts:253](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L253)

#### centroid?

> `optional` **centroid?**: \[`number`, `number`\] \| `null`

#### elevatorCentroid?

> `optional` **elevatorCentroid?**: \[`number`, `number`\] \| `null`

Read-only: centroid of the related location, computed on read.

#### stopPlaceCentroid?

> `optional` **stopPlaceCentroid?**: \[`number`, `number`\] \| `null`

Read-only: centroid of the related location, computed on read.

***

### operational\_status?

> `optional` **operational\_status?**: `"out_of_service"` \| `"unknown"` \| `"operational"` \| `null`

Defined in: [types.ts:230](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L230)

***

### origin\_type?

> `optional` **origin\_type?**: `"operator_reported"` \| `"from_feed"` \| `"manual_entry"` \| `"sensor_detected"` \| `"user_reported"` \| `null`

Defined in: [types.ts:233](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L233)

***

### original\_data?

> `optional` **original\_data?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

Defined in: [types.ts:248](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L248)

***

### original\_elevator\_id?

> `optional` **original\_elevator\_id?**: `string` \| `null`

Defined in: [types.ts:247](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L247)

***

### original\_site\_id?

> `optional` **original\_site\_id?**: `string` \| `null`

Defined in: [types.ts:246](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L246)

***

### pinned?

> `optional` **pinned?**: `boolean` \| `null`

Defined in: [types.ts:235](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L235)

If enabled, this status span will be pinned and given priority over other status spans.

***

### reason\_type?

> `optional` **reason\_type?**: `"maintenance"` \| `"failure"` \| `"under_construction"` \| `"demolition"` \| `"renovation"` \| `"vandalism"` \| `"sensor_jitter"` \| `"not_monitored"` \| `"operation_paused"` \| `null`

Defined in: [types.ts:232](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L232)

***

### related\_spans?

> `optional` **related\_spans?**: ([`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan`)[] \| `null`

Defined in: [types.ts:241](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L241)

Other status spans that are related to this one (linked manually or by feed import logic).

***

### reported\_by?

> `optional` **reported\_by?**: `string` \| `null`

Defined in: [types.ts:244](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L244)

***

### site?

> `optional` **site?**: ([`StopPlaceId`](../type-aliases/StopPlaceId.md) \| [`StopPlace`](StopPlace.md))[] \| `null`

Defined in: [types.ts:225](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L225)

***

### start\_date?

> `optional` **start\_date?**: `string` \| `null`

Defined in: [types.ts:228](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L228)

***

### superseded\_by?

> `optional` **superseded\_by?**: [`StatusSpanId`](../type-aliases/StatusSpanId.md) \| `StatusSpan` \| `null`

Defined in: [types.ts:239](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L239)

The status span that superseded this one (set automatically during imports).

***

### title?

> `optional` **title?**: `string` \| `null`

Defined in: [types.ts:243](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L243)

Automatically generated from description and date range.
