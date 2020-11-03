## [0.2.1] - UNRELEASED

### Bindings Updates
- [November 1, 2020 Vulkan 1.2.159](https://github.com/KhronosGroup/Vulkan-Docs/commit/9adbc1846ddad202a0584f5c03a1916cf9801179)

## [0.2.0] - 2020-10-30

### Bindings Updates
- [October 19, 2020 Vulkan 1.2.158](https://github.com/KhronosGroup/Vulkan-Docs/commit/9fd8fd599b47a67b2eb078b2f5c9e6a2adc922a4)

### Changed
- Changed wrapper methods with possible success codes other than `SUCCESS` or `INCOMPLETE` to return `VkSuccessResult` (new typedef) instead of `VkResult`
- Changed builder methods for void pointers to take references to unconstrained generic types instead (e.g., `&'b mut T` for `*mut c_void`)
- Changed builder methods for opaque arrays (e.g., `*const c_void` with a corresponding length field) to take `u8` slices instead (e.g., `&'b [u8]` for `*const c_void`)

### Added
- Added `SuccessCode` and `ErrorCode` enums
- Added `VkSuccessResult` type alias

## [0.1.0] - 2020-10-19
- Initial release