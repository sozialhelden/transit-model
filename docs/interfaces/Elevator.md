[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / Elevator

# Interface: Elevator

Defined in: types.ts:35

Link elevator infos across data source boundaries.

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "elevators".

## Properties

### capacity\_persons?

> `optional` **capacity\_persons?**: `number` \| `null`

Defined in: types.ts:126

***

### function?

> `optional` **function?**: `object`

Defined in: types.ts:41

Where does this elevator go? Description of the elevator function from the passenger perspective.

#### long\_tts?

> `optional` **long\_tts?**: `string` \| `null`

Long description of the elevator function, e.g. ‘between basement, ground floor, and 1st floor’. Must not contain abbreviations and must be readable aloud.

#### long\_visual?

> `optional` **long\_visual?**: `string` \| `null`

Long description of the elevator function, e.g. ‘between basement, ground floor, and 1st floor to pl. 5’. Can contain abbreviations.

#### short\_tts?

> `optional` **short\_tts?**: `string` \| `null`

Short description of the elevator function, e.g. ‘between basement, ground floor, and 1st floor’. Must not contain abbreviations and must be readable aloud.

#### short\_visual?

> `optional` **short\_visual?**: `string` \| `null`

Short description of the elevator function, e.g. ‘basement ↔ ground floor ↔ 1st floor’. Can contain abbreviations.

***

### holiday\_region?

> `optional` **holiday\_region?**: `object`

Defined in: types.ts:68

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

> `optional` **upcoming\_holidays?**: `string` \| `number` \| `boolean` \| \{\[`k`: `string`\]: `unknown`; \} \| `unknown`[] \| `null`

Next public holidays for the configured region (90 days ahead).

***

### id

> **id**: `number`

Defined in: types.ts:36

***

### internal\_description?

> `optional` **internal\_description?**: `string` \| `null`

Defined in: types.ts:120

***

### linked\_data?

> `optional` **linked\_data?**: `object`

Defined in: types.ts:80

#### alternate\_inventory\_ids?

> `optional` **alternate\_inventory\_ids?**: `object`[] \| `null`

Known alternative inventory IDs for this elevator.

#### associated\_site?

> `optional` **associated\_site?**: [`StopPlaceId`](../type-aliases/StopPlaceId.md) \| [`StopPlace`](StopPlace.md) \| `null`

#### associated\_stops?

> `optional` **associated\_stops?**: [`GtfsStopId`](../type-aliases/GtfsStopId.md)[] \| `null`

GTFS waypoints served by this elevator. Kept in sync with the associated pathways: editing pathways updates this list, and editing this list links/unlinks matching elevator pathways.

#### maintenance\_contact\_missing?

> `optional` **maintenance\_contact\_missing?**: `boolean` \| `null`

#### maintenance\_org?

> `optional` **maintenance\_org?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md) \| `null`

#### monitoring\_unknown?

> `optional` **monitoring\_unknown?**: `boolean` \| `null`

#### nearby\_elevators\_inverse?

> `optional` **nearby\_elevators\_inverse?**: ([`ElevatorId`](../type-aliases/ElevatorId.md) \| `Elevator`)[] \| `null`

#### needs\_review?

> `optional` **needs\_review?**: `boolean` \| `null`

This elevator record needs review and may require updates or verification.

#### no\_realtime\_sensors?

> `optional` **no\_realtime\_sensors?**: `boolean` \| `null`

#### notes?

> `optional` **notes?**: `string` \| `null`

#### obsoleted?

> `optional` **obsoleted?**: `boolean` \| `null`

This elevator record is obsoleted and likely replaced by a newer record from a different data source.

#### operator\_inventory\_id?

> `optional` **operator\_inventory\_id?**: `string` \| `null`

The internal inventory ID used by the operator organization.

#### operator\_is\_unknown?

> `optional` **operator\_is\_unknown?**: `boolean` \| `null`

#### operator\_org?

> `optional` **operator\_org?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md) \| `null`

Responsible for this elevator's function (may be different from the owner).

#### original\_data?

> `optional` **original\_data?**: `string` \| `number` \| `boolean` \| `unknown`[] \| \{\[`k`: `string`\]: `unknown`; \} \| `null`

The original raw data for this elevator from the data source it was imported from

#### original\_site\_id?

> `optional` **original\_site\_id?**: `string` \| `null`

The original site identifier from the data source this elevator was imported from.

#### owner\_is\_unknown?

> `optional` **owner\_is\_unknown?**: `boolean` \| `null`

#### owner\_org?

> `optional` **owner\_org?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md) \| `null`

#### ref?

> `optional` **ref?**: `string` \| `null`

Code for this elevator, e.g. used in local signage.

#### transit\_networks\_served?

> `optional` **transit\_networks\_served?**: ([`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| [`SchemaOrganization`](SchemaOrganization.md))[] \| `null`

***

### location?

> `optional` **location?**: `object`

Defined in: types.ts:52

Where is this elevator located? Description of the elevator location from the passenger perspective.

#### long\_tts?

> `optional` **long\_tts?**: `string` \| `null`

#### long\_visual?

> `optional` **long\_visual?**: `string` \| `null`

Long description of the elevator location, e.g. ‘basement ↔ ground floor ↔ 1st floor’. Can contain abbreviations.

#### short\_tts?

> `optional` **short\_tts?**: `string` \| `null`

Short description of the elevator location, e.g. ‘ground floor ↔ 1st floor’. Must not contain abbreviations. Must be readable aloud.

#### short\_visual?

> `optional` **short\_visual?**: `string` \| `null`

Short description of the elevator location, e.g. ‘ground floor ↔ 1st floor’. Can contain abbreviations.

#### site?

> `optional` **site?**: [`StopPlaceId`](../type-aliases/StopPlaceId.md) \| [`StopPlace`](StopPlace.md) \| `null`

The site where this elevator is located.

***

### nearby?

> `optional` **nearby?**: `object`

Defined in: types.ts:116

#### same\_stop\_place\_elevators?

> `optional` **same\_stop\_place\_elevators?**: ([`ElevatorId`](../type-aliases/ElevatorId.md) \| `Elevator`)[] \| `null`

Other elevator records linked to the same stop place via the “Site” relationship (Where? → Site).

***

### now\_open?

> `optional` **now\_open?**: `boolean` \| `null`

Defined in: types.ts:66

Automatically calculated based on opening hours, current time, and regional public holidays.

***

### number\_of\_doors?

> `optional` **number\_of\_doors?**: `"1"` \| `"2"` \| `null`

Defined in: types.ts:127

***

### opening\_hours?

> `optional` **opening\_hours?**: `string` \| `null`

Defined in: types.ts:64

Example: "Mo-Fr 06:00-22:00; Sa-Su 08:00-20:00; PH off". OSM-compatible format. Use "PH off" to close on public holidays. https://openingh.openstreetmap.de/evaluation_tool/

***

### operational\_status?

> `optional` **operational\_status?**: `object`

Defined in: types.ts:37

#### operational\_status?

> `optional` **operational\_status?**: `"in_service"` \| `"out_of_service"` \| `"partially_operational"` \| `"unknown"` \| `null`

***

### stop\_place\_name?

> `optional` **stop\_place\_name?**: `string` \| `null`

Defined in: types.ts:129

Computed field combining the stop name and description for easier searching.

***

### url?

> `optional` **url?**: `object`[] \| `null`

Defined in: types.ts:121
