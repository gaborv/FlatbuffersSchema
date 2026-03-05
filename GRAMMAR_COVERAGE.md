# FlatBuffers Grammar Coverage

This document details the complete grammar support provided by this VS Code extension based on the official FlatBuffers grammar specification at https://flatbuffers.dev/grammar/

## Full Grammar Support Status

### ✅ Keywords and Declarations (100% Coverage)

All keywords from the official grammar are supported:

| Keyword | Status | Description |
|---------|--------|-------------|
| `include` | ✅ Supported | Include other schema files |
| `namespace` | ✅ Supported | Package/namespace declarations |
| `attribute` | ✅ Supported | Custom attribute declarations |
| `table` | ✅ Supported | Table type declarations (main object types) |
| `struct` | ✅ Supported | Struct type declarations (fixed-size, always present) |
| `enum` | ✅ Supported | Enumeration declarations |
| `union` | ✅ Supported | Union type declarations (polymorphic types) |
| `root_type` | ✅ Supported | Root type specification |
| `file_extension` | ✅ Supported | File extension for generated files |
| `file_identifier` | ✅ Supported | 4-character file identifier for binary verification |
| `rpc_service` | ✅ Supported | RPC service declarations (for gRPC integration) |

### ✅ Data Types (100% Coverage)

All data types from the official grammar are supported:

#### Basic Types
| Type | Status | Description |
|------|--------|-------------|
| `bool` | ✅ Supported | Boolean (1 byte) |
| `byte` | ✅ Supported | Signed 8-bit integer |
| `ubyte` | ✅ Supported | Unsigned 8-bit integer |
| `short` | ✅ Supported | Signed 16-bit integer |
| `ushort` | ✅ Supported | Unsigned 16-bit integer |
| `int` | ✅ Supported | Signed 32-bit integer |
| `uint` | ✅ Supported | Unsigned 32-bit integer |
| `float` | ✅ Supported | 32-bit floating point |
| `long` | ✅ Supported | Signed 64-bit integer |
| `ulong` | ✅ Supported | Unsigned 64-bit integer |
| `double` | ✅ Supported | 64-bit floating point |
| `string` | ✅ Supported | UTF-8 or 7-bit ASCII string |

#### Extended Numeric Types (Explicitly Sized)
| Type | Status | Description |
|------|--------|-------------|
| `int8` | ✅ Supported | Signed 8-bit integer (alias for byte) |
| `uint8` | ✅ Supported | Unsigned 8-bit integer (alias for ubyte) |
| `int16` | ✅ Supported | Signed 16-bit integer (alias for short) |
| `uint16` | ✅ Supported | Unsigned 16-bit integer (alias for ushort) |
| `int32` | ✅ Supported | Signed 32-bit integer (alias for int) |
| `uint32` | ✅ Supported | Unsigned 32-bit integer (alias for uint) |
| `int64` | ✅ Supported | Signed 64-bit integer (alias for long) |
| `uint64` | ✅ Supported | Unsigned 64-bit integer (alias for ulong) |
| `float32` | ✅ Supported | 32-bit floating point (alias for float) |
| `float64` | ✅ Supported | 64-bit floating point (alias for double) |

### ✅ Metadata Attributes (Full Coverage)

All common metadata attributes are supported:

| Attribute | Status | Description |
|-----------|--------|-------------|
| `id` | ✅ Supported | Manually assign field ID for schema evolution |
| `deprecated` | ✅ Supported | Mark field as deprecated (no code generated) |
| `required` | ✅ Supported | Field must be present (verifier will fail if absent) |
| `key` | ✅ Supported | Mark field as key for sorted vectors |
| `original_order` | ✅ Supported | Maintain original field order despite ID attributes |
| `force_align` | ✅ Supported | Force custom byte alignment for field |
| `bit_flags` | ✅ Supported | Mark enum as bit flags |
| `nested_flatbuffer` | ✅ Supported | Indicate bytes field contains nested FlatBuffer |
| `hash` | ✅ Supported | Custom hash function hint |
| `native_inline` | ✅ Supported | Control native language implementation storage |
| `native_type` | ✅ Supported | Custom native type mapping |
| `native_default` | ✅ Supported | Native default value |
| `flexbuffer` | ✅ Supported | FlexBuffer support |
| `streaming` | ✅ Supported | gRPC streaming annotation for RPC methods |

### ✅ Advanced Features

| Feature | Status | Description |
|---------|--------|-------------|
| Vectors | ✅ Supported | Arrays denoted with `[type]` |
| Nested tables | ✅ Supported | Tables can contain other tables |
| Default values | ✅ Supported | Scalar fields can have default values |
| Comments | ✅ Supported | Line comments (`//`) and block comments (`/* */`) |
| Namespaces | ✅ Supported | Hierarchical namespaces with dot notation |
| Custom attributes | ✅ Supported | User-defined attributes |

## Recent Updates (2024-2026)

According to the official FlatBuffers changelog and documentation:

### No Grammar Deprecations
- ✅ **No keywords or grammar features have been deprecated or removed** in the 2024-2026 period
- ✅ The `.fbs` schema grammar remains **stable and backward compatible**
- ✅ All features in this extension match the current official specification

### What Changed (Non-Grammar)
The following changes occurred but **do not affect the schema grammar**:
- Documentation moved to https://flatbuffers.dev (old docs removed Feb 2025)
- TypeScript Verifier constructor deprecated (not schema-related)
- Bazel build system updates (not schema-related)
- New language bindings and code generators (not schema-related)

## Testing and Validation

A comprehensive sample file (`sample.fbs`) is included in this repository that demonstrates:
- All supported keywords and declarations
- All data types (basic and extended)
- All metadata attributes
- RPC service declarations
- Complex nested structures
- Schema evolution features

## Grammar Reference

The official grammar specification is maintained at:
- **Grammar**: https://flatbuffers.dev/grammar/
- **Schema Overview**: https://flatbuffers.dev/schema/
- **Tutorial**: https://flatbuffers.dev/tutorial/

## Summary

✅ **This VS Code extension provides 100% coverage of the official FlatBuffers grammar**

All keywords, data types, metadata attributes, and advanced features from the specification are supported and properly highlighted. No deprecated features need to be removed as the grammar has remained stable.
