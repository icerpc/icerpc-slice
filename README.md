# IceRPC Slice files

This directory provides [Slice] definitions shared by all IceRPC implementations.

| Subdirectory       | Description                                                                                                                                                                                                                                                                    |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| IceRpc             | Types provided by all IceRPC implementations. These types are IceRPC-specific.                                                                                                                                                                                                 |
| IceRpc/Ice         | Types and interfaces provided for interop with [Ice] applications. They are defined using Ice's [original Slice language][Ice Slice].                                                                                                                                          |
| IceRpc/**/Internal | Types used by IceRPC implementations to implement the [ice][ice-protocol] protocol, the [icerpc][icerpc-protocol] protocol, the [Slic] protocol and more. These are internal IceRPC implementation details—applications built with IceRPC don't need to see these definitions. |
| WellKnownTypes     | Custom types such as Uri and TimeStamp. These well-known types are RPC-independent.                                                                                                                                                                                            |

The copy of record for these Slice files is in this repository. Each IceRPC implementation is expected to create its
own exact clone of these Slice files. For example, see the [sync-slice.py] Python script in icerpc-csharp.

[Ice]: https://github.com/zeroc-ice/ice
[Ice Slice]: https://docs.zeroc.com/ice/3.8/cpp/the-slice-language
[ice-protocol]: https://docs.icerpc.dev/icerpc/ice-protocol/protocol-frames
[icerpc-protocol]: https://docs.icerpc.dev/icerpc/icerpc-protocol/mapping-rpcs-to-streams
[Slic]: https://docs.icerpc.dev/icerpc/slic-transport/protocol-frames
[Slice]: https://docs.icerpc.dev/slice
[sync-slice.py]: https://github.com/icerpc/icerpc-csharp/blob/main/build/sync-slice.py
