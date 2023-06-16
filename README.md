# IceRPC Slice files

This repository, [icerpc-slice][icerpc-slice], provides [Slice][slice] files shared by all IceRPC implementations.

| Directory      | Description |
|----------------|-------------|
| Ice            | Interfaces and structs in module Ice, provided for interop with [Ice][zeroc-ice] applications.|
| IceRpc         | Enumerations that specify response status codes, request field keys, response field keys and known compression formats.|
| WellKnownTypes | Custom types supported by all IceRPC implementations.|
| **/Internal    | Enumerations and compact structs used by IceRPC implementations to implement the [icerpc][icerpc-protocol] protocol, the [ice][ice-protocol] protocol, the Slice [encoding][slice-encoding] and the [Slic][slic] multiplexing adapter. These are internal IceRPC implementation details—applications that use IceRPC don't need to see these definitions.|

> **Note**
> Each IceRPC implementation is expected to create a git subtree with a copy of this repository. For example, the
> `slice` directory of the [icerpc-csharp][icerpc-csharp] repository is a git subtree copy of this repository.

[ice-protocol]: https://docs.testing.zeroc.com/docs/icerpc-core/ice-protocol/protocol-frames
[icerpc-csharp]: https://github.com/icerpc/icerpc-csharp/
[icerpc-protocol]: https://docs.testing.zeroc.com/docs/icerpc-core/icerpc-protocol/mapping-rpcs-to-streams
[icerpc-slice]: https://github.com/icerpc/icerpc-slice
[slic]: TBD
[slice]: https://docs.testing.zeroc.com/docs/slice
[slice-encoding]: https://docs.testing.zeroc.com/docs/slice/encoding/main-features
[zeroc-ice]: https://github.com/zeroc-ice/ice
