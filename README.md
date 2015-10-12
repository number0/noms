# Noms

Noms is a content-addressable, immutable, peer-to-peer datastore for structured data.

In other words, *noms is git for data*.

This repository will contain the reference implementation of the noms protocol, and will eventually be open sourced. 

This includes:

* Go wrappers for all the core noms types
* Support for generating Go types from Nom schema definitions
* Chunking and dechunking
* Serialization and deserialization
* Chunkstore interface as well as several sample implementations
* Search support
* Sample applications

# Get the code

```
git clone https://github.com/attic-labs/noms
```

# Build

```
go build ./...
go test ./...
```

# Run

```
cd <noms>/clients/counter
go build
./counter -ldb=/tmp/foo -ds=foo
./counter -ldb=/tmp/foo -ds=foo
./counter -ldb=/tmp/foo -ds=foo
```

rejoice!

You can see the raw data:

```
ls /tmp/foo
cat /tmp/foo/*.log | strings
```

You can also explore the data visually. Follow the instructions in `clients/explore`.
