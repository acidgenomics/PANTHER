## PANTHER 0.2.1 (2021-03-12)

### Minor changes

- Updated basejump dependencies, and removed now unnecessary stringr import.

## PANTHER 0.2.0 (2021-03-02)

### Major changes

- Simplified internal code, using improved methods defined in basejump v0.14
  release series. In particular, now taking advantage of `CharacterList`
  methods for operations on list columns, which are way faster than attempting
  to process via BiocParallel.
- Updated to support PANTHER 16.0, which has introduced some breaking changes.

## PANTHER 0.1.4 (2020-10-28)

### Minor changes

- Improved message consistency, using cli package.
- Sped up package checks for Travis CI inside Docker image.

## PANTHER 0.1.3 (2020-10-12)

### Minor changes

- Updated basejump dependencies.

## PANTHER 0.1.2 (2020-07-23)

### Minor changes

- Maintenance release, upgrading R dependency to 4.0.

## PANTHER 0.1.1 (2020-01-08)

### Minor changes

- Documentation updates, using roxygen2 7.0 release.
- Bug fix in transformer `mutateAll` required, for improved nested list column
  handling following Bioconductor update. Added an internal `as_tibble()` call
  prior to handoff to `DataFrame`, which improves return consistency for nested
  list columns.

## PANTHER 0.1.0 (2019-09-25)

Initial release. Code was split out from basejump package.
