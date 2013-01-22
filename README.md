Welcome to Hibari. Hibari is a production-ready, distributed,
key-value, big data store. Hibari uses chain replication for strong
consistency, high-availability, and durability. Hibari has excellent
performance especially for read and large value operations.


# Quick Start

Please read Getting Started section of Hibari Application Developer Guide.

- [English Version](http://hibari.github.com/hibari-doc/hibari-app-developer-guide.en.html#getting-started)
- [Japanese Version](http://hibari.github.com/hibari-doc/hibari-app-developer-guide.ja.html#getting-started)


# Hibari Documentation

- [English Version](http://hibari.github.com/hibari-doc/)
- [Japanese Version](http://hibari.github.com/hibari-doc/)


# Hibari Mailing Lists

- [Google Group **hibaridb-users** for English Speakers](http://groups.google.com/forum/#!forum/hibaridb-users)
- [Google Group **hibaridb-users-ja** for Japanese Speakers](http://groups.google.com/forum/#!forum/hibaridb-users-ja)


# Roadmap

Short-term roadmap

## v0.1 series (unstable)

- v0.1.10
  * Minor bug fixes
  * Update for Erlang/OTP R15
  * Support for building on Ubuntu, including ARMv7 architecture
  * Move S3 and JSON-RPC components out from Hibari distribution
    (remove from the `repo` manifests.)  S3 and JSON-RPC will become
    separate projects and will use `rebar` to manage
    dependencies. (Hibari will continue using `repo`)


## v0.5 series (unstable)

- v0.5
  * A complete Thrift API (`do`, `get_many`, and `testset` flag for
    `set` and `replace`)
  * Server-side timestamp and rename (Server-side timestamp is
    required by Thrift API)
  * Server-side counter
  * Basho Bench driver


## v0.6 series (stable)

- v0.6
  * Source code package. Application developers can build Hibari
    without `repo` by using this package. (Hibari developers will
    continue using `repo`.)
  * Documentation rework
  * Sample codes
  * Cookbook for Opscode Chef for automated single-node and multi-node
    deployments
  * More QuickCheck and EUnit test cases


## Unscheduled Features

- MapReduce (mruby?)
- SNMP support
- LETS (Google LevelDB) or HanoiDB as an alternative key storage for
  optimizing RAM usage
- Scavenger enhancements
- Big writes/reads (`append` to a value and `partial_read` from a value)


_EOF_