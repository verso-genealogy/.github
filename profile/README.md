# Verso

**Genealogical records of the Russian Empire, written as code.**

[По-русски →](https://github.com/verso-genealogy/.github/blob/main/profile/README.ru.md)

Parish metric books, revision lists (ревизские сказки), confession lists (исповедные росписи):
each record is typed once, as the scribe wrote it, as a call of a small Python DSL — one file per
book and year, names in the original orthography. From those files Verso builds Geni profiles
(as Terraform), Familio справочники, CSV and a records JSON.

Unlike a spreadsheet, a record here is read back and checked before it is published; unlike
typing straight into a family-tree site, the source stays the one text everything else is
derived from.

## What the checks catch

Once the records of a village are in, Verso reads them all together and points to what they
contradict:

- a wedding dated to a day the Church did not marry on, such as a fast;
- a death record whose stated age disagrees with the same child's birth record;
- two children of one couple born impossibly close together;
- a christening, death or burial dated before an earlier event of the same life.

Each finding names the records it comes from, so it is checked against the scan, not taken on
trust.

## Repositories

| | |
|---|---|
| [**verso**](https://github.com/verso-genealogy/verso) | The library: the DSL, its linters, the checks, the exporters to Geni, Familio, CSV and JSON. Apache-2.0. |

## Start here

- [Quick start](https://github.com/verso-genealogy/verso#quick-start) — a toy village, run end to end
- [The DSL](https://github.com/verso-genealogy/verso/blob/main/docs/dsl.md) ·
  [Commands](https://github.com/verso-genealogy/verso/blob/main/docs/reference/commands.md)
- [Contributing](https://github.com/verso-genealogy/verso/blob/main/CONTRIBUTING.md) ·
  [Security](https://github.com/verso-genealogy/verso/security)
