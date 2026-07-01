[**@sozialhelden/transit-model**](../README.md)

***

[@sozialhelden/transit-model](../README.md) / SchemaOrganization

# Interface: SchemaOrganization

Defined in: types.ts:236

This interface was referenced by `Config`'s JSON-Schema
via the `definition` "schema-organizations".

## Properties

### \_autoSuggestion?

> `optional` **\_autoSuggestion?**: `object`

Defined in: types.ts:358

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

Defined in: types.ts:357

MongoDB source _id values from the old accessibility.cloud database that belong to this organization.

***

### address?

> `optional` **address?**: `object`

Defined in: types.ts:249

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

Defined in: types.ts:240

***

### belongs\_to\_transit\_network?

> `optional` **belongs\_to\_transit\_network?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| `SchemaOrganization` \| `null`

Defined in: types.ts:267

***

### branding?

> `optional` **branding?**: `object`

Defined in: types.ts:304

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

Defined in: types.ts:258

***

### country

> **country**: `string`

Defined in: types.ts:257

ISO 3166-1 ALPHA-2, e.g., "UA" (Ukraine), "FR" (France), "US" (United States), "NZ" (New Zealand)

***

### description?

> `optional` **description?**: `string` \| `null`

Defined in: types.ts:244

***

### generateSlug?

> `optional` **generateSlug?**: `boolean` \| `null`

Defined in: types.ts:247

When enabled, the slug will auto-generate from the title field on save and autosave.

***

### id

> **id**: `number`

Defined in: types.ts:237

***

### legalName?

> `optional` **legalName?**: `string` \| `null`

Defined in: types.ts:239

***

### name

> **name**: `string`

Defined in: types.ts:238

***

### netexAuthorityRef?

> `optional` **netexAuthorityRef?**: `string` \| `null`

Defined in: types.ts:352

***

### notes?

> `optional` **notes?**: `string` \| `null`

Defined in: types.ts:245

***

### operationalStatus?

> `optional` **operationalStatus?**: `"planned"` \| `"active"` \| `"inactive"` \| `"suspended"` \| `null`

Defined in: types.ts:264

***

### organizationType

> **organizationType**: `"transport_authority"` \| `"public_transport_operator"` \| `"public_transport_operator_national"` \| `"data_publisher"` \| `"technology_provider"` \| `"research_institution"` \| `"government_agency"` \| `"interest_group"`

Defined in: types.ts:266

***

### osmManufacturerName?

> `optional` **osmManufacturerName?**: `string` \| `null`

Defined in: types.ts:355

***

### osmNetworkName?

> `optional` **osmNetworkName?**: `string` \| `null`

Defined in: types.ts:354

***

### osmOperatorName?

> `optional` **osmOperatorName?**: `string` \| `null`

Defined in: types.ts:353

***

### parentOrganization?

> `optional` **parentOrganization?**: [`SchemaOrganizationId`](../type-aliases/SchemaOrganizationId.md) \| `SchemaOrganization` \| `null`

Defined in: types.ts:265

***

### preferredIconographies?

> `optional` **preferredIconographies?**: [`IconographyId`](../type-aliases/IconographyId.md)[] \| `null`

Defined in: types.ts:303

Iconographies this organization prefers, in order.

***

### providedTransportModes?

> `optional` **providedTransportModes?**: [`TransitModeId`](../type-aliases/TransitModeId.md)[] \| `null`

Defined in: types.ts:348

Means of transport this organization provides.

***

### slug

> **slug**: `string`

Defined in: types.ts:248

***

### status\_templates?

> `optional` **status\_templates?**: `object`

Defined in: types.ts:268

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

Defined in: types.ts:346

***

### url?

> `optional` **url?**: `string` \| `null`

Defined in: types.ts:349

***

### wikidataId?

> `optional` **wikidataId?**: `string` \| `null`

Defined in: types.ts:351

Link to the corresponding Wikidata entity (e.g., https://www.wikidata.org/entity/Q12345).
