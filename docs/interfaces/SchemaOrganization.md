[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / SchemaOrganization

# Interface: SchemaOrganization

Defined in: [types.ts:266](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L266)

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "schema-organizations".

## Properties

### \_autoSuggestion?

> `optional` **\_autoSuggestion?**: `object`

Defined in: [types.ts:392](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L392)

#### appliedAt?

> `optional` **appliedAt?**: `string` \| `null`

#### pluginId?

> `optional` **pluginId?**: `string` \| `null`

#### suggestionId?

> `optional` **suggestionId?**: `string` \| `null`

#### title?

> `optional` **title?**: `string` \| `null`

***

### acLegacySourceIds?

> `optional` **acLegacySourceIds?**: `string`[] \| `null`

Defined in: [types.ts:391](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L391)

MongoDB source _id values from the old accessibility.cloud database that belong to this organization.

***

### address?

> `optional` **address?**: `object`

Defined in: [types.ts:279](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L279)

#### addressCountry?

> `optional` **addressCountry?**: `string` \| `null`

#### addressLocality?

> `optional` **addressLocality?**: `string` \| `null`

#### addressRegion?

> `optional` **addressRegion?**: `string` \| `null`

#### postalCode?

> `optional` **postalCode?**: `string` \| `null`

#### streetAddress?

> `optional` **streetAddress?**: `string` \| `null`

***

### alternateName?

> `optional` **alternateName?**: `object`[] \| `null`

Defined in: [types.ts:270](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L270)

***

### belongs\_to\_transit\_network?

> `optional` **belongs\_to\_transit\_network?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| `SchemaOrganization` \| `null`

Defined in: [types.ts:297](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L297)

***

### branding?

> `optional` **branding?**: `object`

Defined in: [types.ts:338](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L338)

#### darkAccentColor?

> `optional` **darkAccentColor?**: `string` \| `null`

CSS color value

#### darkBackgroundColorGrayscale?

> `optional` **darkBackgroundColorGrayscale?**: `string` \| `null`

CSS color value

#### darkBackgroundColorMuted?

> `optional` **darkBackgroundColorMuted?**: `string` \| `null`

CSS color value

#### darkBackgroundColorTinted?

> `optional` **darkBackgroundColorTinted?**: `string` \| `null`

CSS color value

#### darkPrimaryColor?

> `optional` **darkPrimaryColor?**: `string` \| `null`

CSS color value

#### deduplicateIconAndName?

> `optional` **deduplicateIconAndName?**: `boolean` \| `null`

#### deduplicateLogoAndName?

> `optional` **deduplicateLogoAndName?**: `boolean` \| `null`

#### iconDark?

> `optional` **iconDark?**: [`MediaId`](../type-aliases/MediaId.md) \| `null`

SVG preferred. Squared image for compact contexts (favicons, map markers).

#### iconDarkOptimized?

> `optional` **iconDarkOptimized?**: `string` \| `null`

Auto-filled with the SVGO-optimized SVG markup when an SVG icon is uploaded.

#### iconLight?

> `optional` **iconLight?**: [`MediaId`](../type-aliases/MediaId.md) \| `null`

SVG preferred. Squared image for compact contexts (favicons, map markers).

#### iconLightOptimized?

> `optional` **iconLightOptimized?**: `string` \| `null`

Auto-filled with the SVGO-optimized SVG markup when an SVG icon is uploaded.

#### iconWorksOnAllBackgrounds?

> `optional` **iconWorksOnAllBackgrounds?**: `boolean` \| `null`

#### lightAccentColor?

> `optional` **lightAccentColor?**: `string` \| `null`

CSS color value

#### lightBackgroundColorGrayscale?

> `optional` **lightBackgroundColorGrayscale?**: `string` \| `null`

CSS color value

#### lightBackgroundColorMuted?

> `optional` **lightBackgroundColorMuted?**: `string` \| `null`

CSS color value

#### lightBackgroundColorTinted?

> `optional` **lightBackgroundColorTinted?**: `string` \| `null`

CSS color value

#### lightPrimaryColor?

> `optional` **lightPrimaryColor?**: `string` \| `null`

CSS color value

#### logoDark?

> `optional` **logoDark?**: [`MediaId`](../type-aliases/MediaId.md) \| `null`

SVG preferred. Used where the full organization or app name is displayed.

#### logoDarkOptimized?

> `optional` **logoDarkOptimized?**: `string` \| `null`

Auto-filled with the SVGO-optimized SVG markup when an SVG logo is uploaded.

#### logoLight?

> `optional` **logoLight?**: [`MediaId`](../type-aliases/MediaId.md) \| `null`

SVG preferred. Used where the full organization or app name is displayed.

#### logoLightOptimized?

> `optional` **logoLightOptimized?**: `string` \| `null`

Auto-filled with the SVGO-optimized SVG markup when an SVG logo is uploaded.

#### logoWorksOnAllBackgrounds?

> `optional` **logoWorksOnAllBackgrounds?**: `boolean` \| `null`

***

### contactPoint?

> `optional` **contactPoint?**: `object`[] \| `null`

Defined in: [types.ts:288](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L288)

***

### country

> **country**: `string`

Defined in: [types.ts:287](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L287)

ISO 3166-1 ALPHA-2, e.g., "UA" (Ukraine), "FR" (France), "US" (United States), "NZ" (New Zealand)

***

### description?

> `optional` **description?**: `string` \| `null`

Defined in: [types.ts:274](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L274)

***

### generateSlug?

> `optional` **generateSlug?**: `boolean` \| `null`

Defined in: [types.ts:277](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L277)

When enabled, the slug will auto-generate from the title field on save and autosave.

***

### id

> **id**: `number`

Defined in: [types.ts:267](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L267)

***

### legalName?

> `optional` **legalName?**: `string` \| `null`

Defined in: [types.ts:269](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L269)

***

### name

> **name**: `string`

Defined in: [types.ts:268](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L268)

***

### netexAuthorityRef?

> `optional` **netexAuthorityRef?**: `string` \| `null`

Defined in: [types.ts:386](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L386)

***

### notes?

> `optional` **notes?**: `string` \| `null`

Defined in: [types.ts:275](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L275)

***

### operationalStatus?

> `optional` **operationalStatus?**: `"planned"` \| `"active"` \| `"inactive"` \| `"suspended"` \| `null`

Defined in: [types.ts:294](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L294)

***

### organizationType

> **organizationType**: `"transport_authority"` \| `"public_transport_operator"` \| `"public_transport_operator_national"` \| `"data_publisher"` \| `"technology_provider"` \| `"research_institution"` \| `"government_agency"` \| `"interest_group"`

Defined in: [types.ts:296](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L296)

***

### osmManufacturerName?

> `optional` **osmManufacturerName?**: `string` \| `null`

Defined in: [types.ts:389](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L389)

***

### osmNetworkName?

> `optional` **osmNetworkName?**: `string` \| `null`

Defined in: [types.ts:388](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L388)

***

### osmOperatorName?

> `optional` **osmOperatorName?**: `string` \| `null`

Defined in: [types.ts:387](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L387)

***

### parentOrganization?

> `optional` **parentOrganization?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| `SchemaOrganization` \| `null`

Defined in: [types.ts:295](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L295)

***

### preferredIconographies?

> `optional` **preferredIconographies?**: [`IconographyId`](../type-aliases/IconographyId.md)[] \| `null`

Defined in: [types.ts:337](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L337)

Iconographies this organization prefers, in order.

***

### providedTransportModes?

> `optional` **providedTransportModes?**: ([`TransitModeId`](../type-aliases/TransitModeId.md) \| [`TransitMode`](TransitMode.md))[] \| `null`

Defined in: [types.ts:382](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L382)

Means of transport this organization provides.

***

### slug

> **slug**: `string`

Defined in: [types.ts:278](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L278)

***

### status\_templates?

> `optional` **status\_templates?**: `object`

Defined in: [types.ts:298](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L298)

#### demolition\_generic?

> `optional` **demolition\_generic?**: `string` \| `null`

#### demolition\_generic\_short?

> `optional` **demolition\_generic\_short?**: `string` \| `null`

#### demolition\_with\_location?

> `optional` **demolition\_with\_location?**: `string` \| `null`

#### demolition\_with\_location\_short?

> `optional` **demolition\_with\_location\_short?**: `string` \| `null`

#### long\_term\_generic?

> `optional` **long\_term\_generic?**: `string` \| `null`

#### long\_term\_generic\_short?

> `optional` **long\_term\_generic\_short?**: `string` \| `null`

#### long\_term\_with\_location?

> `optional` **long\_term\_with\_location?**: `string` \| `null`

#### long\_term\_with\_location\_short?

> `optional` **long\_term\_with\_location\_short?**: `string` \| `null`

#### maintenance\_generic?

> `optional` **maintenance\_generic?**: `string` \| `null`

#### maintenance\_generic\_short?

> `optional` **maintenance\_generic\_short?**: `string` \| `null`

#### maintenance\_with\_location?

> `optional` **maintenance\_with\_location?**: `string` \| `null`

#### maintenance\_with\_location\_short?

> `optional` **maintenance\_with\_location\_short?**: `string` \| `null`

#### not\_monitored\_generic?

> `optional` **not\_monitored\_generic?**: `string` \| `null`

#### not\_monitored\_generic\_short?

> `optional` **not\_monitored\_generic\_short?**: `string` \| `null`

#### not\_monitored\_with\_location?

> `optional` **not\_monitored\_with\_location?**: `string` \| `null`

#### not\_monitored\_with\_location\_short?

> `optional` **not\_monitored\_with\_location\_short?**: `string` \| `null`

#### operation\_paused\_generic?

> `optional` **operation\_paused\_generic?**: `string` \| `null`

#### operation\_paused\_generic\_short?

> `optional` **operation\_paused\_generic\_short?**: `string` \| `null`

#### operation\_paused\_with\_location?

> `optional` **operation\_paused\_with\_location?**: `string` \| `null`

#### operation\_paused\_with\_location\_short?

> `optional` **operation\_paused\_with\_location\_short?**: `string` \| `null`

#### renovation\_generic?

> `optional` **renovation\_generic?**: `string` \| `null`

#### renovation\_generic\_short?

> `optional` **renovation\_generic\_short?**: `string` \| `null`

#### renovation\_with\_location?

> `optional` **renovation\_with\_location?**: `string` \| `null`

#### renovation\_with\_location\_short?

> `optional` **renovation\_with\_location\_short?**: `string` \| `null`

#### sensor\_jitter\_generic?

> `optional` **sensor\_jitter\_generic?**: `string` \| `null`

#### sensor\_jitter\_generic\_short?

> `optional` **sensor\_jitter\_generic\_short?**: `string` \| `null`

#### sensor\_jitter\_with\_location?

> `optional` **sensor\_jitter\_with\_location?**: `string` \| `null`

#### sensor\_jitter\_with\_location\_short?

> `optional` **sensor\_jitter\_with\_location\_short?**: `string` \| `null`

#### short\_outage\_generic?

> `optional` **short\_outage\_generic?**: `string` \| `null`

#### short\_outage\_generic\_short?

> `optional` **short\_outage\_generic\_short?**: `string` \| `null`

#### short\_outage\_with\_location?

> `optional` **short\_outage\_with\_location?**: `string` \| `null`

#### short\_outage\_with\_location\_short?

> `optional` **short\_outage\_with\_location\_short?**: `string` \| `null`

#### vandalism\_generic?

> `optional` **vandalism\_generic?**: `string` \| `null`

#### vandalism\_generic\_short?

> `optional` **vandalism\_generic\_short?**: `string` \| `null`

#### vandalism\_with\_location?

> `optional` **vandalism\_with\_location?**: `string` \| `null`

#### vandalism\_with\_location\_short?

> `optional` **vandalism\_with\_location\_short?**: `string` \| `null`

***

### transportModes?

> `optional` **transportModes?**: (`"bus"` \| `"tram"` \| `"metro"` \| `"rail"` \| `"ferry"` \| `"cable_car"` \| `"funicular"` \| `"monorail"` \| `"aerial_lift"` \| `"shared_mobility"` \| `"e_scooter"` \| `"bike"` \| `"car"`)[] \| `null`

Defined in: [types.ts:380](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L380)

***

### url?

> `optional` **url?**: `string` \| `null`

Defined in: [types.ts:383](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L383)

***

### wikidataId?

> `optional` **wikidataId?**: `string` \| `null`

Defined in: [types.ts:385](https://github.com/sozialhelden/transit-model/blob/c678a5dad27639a9ad98b54bd5467e529bc11aec/src/types.ts#L385)

Link to the corresponding Wikidata entity (e.g., https://www.wikidata.org/entity/Q12345).
