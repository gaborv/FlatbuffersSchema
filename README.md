# Flatbuffers Schema colorizer for Visual Studio Code
This simple language support module provides syntax highlighting for FlatBuffers schema definition files (.fbs).

More about the Flatbuffers schema: https://flatbuffers.dev/schema/

## Features

- ✅ **Full Grammar Support** - 100% coverage of the official FlatBuffers grammar specification
- ✅ **All Data Types** - Support for all basic and extended numeric types (int8, uint8, int16, uint16, int32, uint32, int64, uint64, float32, float64)
- ✅ **RPC Services** - Complete support for `rpc_service` declarations for gRPC integration
- ✅ **Metadata Attributes** - All standard and custom metadata attributes
- ✅ **Modern Syntax** - Up-to-date with the latest FlatBuffers specification

## Sample File

See [sample.fbs](./sample.fbs) for a comprehensive example demonstrating all supported grammar features.

## Grammar Coverage

For detailed information about grammar support, see [GRAMMAR_COVERAGE.md](./GRAMMAR_COVERAGE.md).

## References

- Official Grammar: https://flatbuffers.dev/grammar/
- Schema Documentation: https://flatbuffers.dev/schema/
- FlatBuffers Tutorial: https://flatbuffers.dev/tutorial/

## Acknowledgements
I used the grammar file from [Tobias Kahlert's Flatbuffers plugin for Atom](https://github.com/SrTobi/language-flatbuffers) and converted it to JSON to use it here. The grammar has been extended to support the full modern FlatBuffers specification.

