# @sozialhelden/transit-model

Public, minimal data model for the **Wheelmap Transit** API: the four consumer-facing
collections — **Elevator**, **StopPlace**, **StatusSpan**, **SchemaOrganization**.

It carries only field **names + descriptions + types**. No hooks, no audit/system fields
(`createdAt`, `updatedAt`, `deletedAt`, `_status`, `feed`, `feed_import`, …), no internals.

> `src/types.ts` and `src/tables.ts` are **auto-generated** from the transit app's
> `payload-types.ts` / `payload-generated-schema.ts` by `scripts/generate-transit-model.ts`.
> Do not edit them by hand.

## Install

```bash
npm install @sozialhelden/transit-model
# or
pnpm add @sozialhelden/transit-model
```

## Types

Each relationship field uses a **branded ID** that also accepts the referenced entity:

```ts
import type { Elevator, StopPlaceId } from '@sozialhelden/transit-model';

const elevator: Elevator = {
  id: 7037,
  location: {
    // accepts a branded id, the full entity, or null
    site: { id: 42, /* …StopPlace… */ } as StopPlace | StopPlaceId | null,
  },
  // …
};
```

`Id<Brand>` is a `number` branded with its collection, so a branded id is assignable to any
`number` parameter, while a plain `number` must be branded first (prevents mixing up e.g. a
`StopPlaceId` with a `SchemaOrganizationId`). Use the `asId` helper to brand a raw id:

```ts
import { asId } from '@sozialhelden/transit-model';

const site = asId<'StopPlace'>(42); // StopPlaceId
```

## Table model

A dependency-free description of each collection's physical columns
(`dbColumn`, `sqlType`, `tsType`, `nullable`, `enumValues`, `references`):

```ts
import { tables } from '@sozialhelden/transit-model';

tables.elevators.columns;
// [{ dbColumn: 'location_site_id', sqlType: 'integer', tsType: 'StopPlaceId', nullable: true, … }, …]
```

Only the main physical table of each collection is described (localized fields live in
separate `*_locales` tables and are intentionally not included).

## Build / regenerate

From the transit app:

```bash
pnpm generate:model          # regenerate src/*.ts + build dist + docs
pnpm generate:types          # regenerates payload-types.ts, which triggers postgenerate:types -> generate:model
pnpm build                   # app build, which triggers postbuild -> generate:model
```

The Markdown API docs in `docs/` are produced by TypeDoc (`typedoc-plugin-markdown`) and are
committed.
