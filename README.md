# awesome-serialization [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> So many formats, so little bandwidth.  *See [wesm](https://github.com/18F/data-act-pilot/issues/161#issuecomment-139812420) comment before making up your mind.*

## Contents

- [API](#api)
- [RPC](#rpc)
- [Big Data](#big-data)
- [Scientific](#scientific)
- [Machine Learning](#machine-learning)
- [Graph](#graph)
- [Object](#object)
- [Workflow](#workflow)
- [Programming](#programming)
- [Academic](#academic)

## API

Serialization suitible for API RPC networked services.

- [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) - Comma Separated Values. Textual.
- [JSON](https://www.json.org) - Lightweight document data-interchange format. Textual.
- [JSONL](https://jsonlines.org) - Schemeless "multiple JSON documents in 1 file" container data format. Textual.
- [Thrift](http://thrift.apache.org) - Scalable code generation, schema evolution binary format. Binary.
- [Protocol Buffers](https://github.com/protocolbuffers/protobuf) - Google's data interchange format. Binary.
- [Message Pack](https://msgpack.org) - Efficient JSON-like binary serialization format. Binary.
- [bson](http://bsonspec.org) - Binary schemeless JSON encoding. Binary.
- [XML](https://www.w3.org/XML/) - Extensible Markup Language. Genuinely Horrible. Textual.
- [Plist](https://en.wikipedia.org/wiki/Property_list) - Property List representation. Apple. Textual.
- [YAML](https://yaml.org) - Identation based data serialization standard. Textual.
- [TOML](https://github.com/toml-lang/toml) - Tom's Obvious, Minimal Language. Textual.

## RPC

 - [gRPC](https://grpc.io) - A high-performance, open source universal RPC framework. Binary, ISO Layer 7.
 - [RSocket](https://rsocket.io) - Application protocol providing Reactive Streams semantics. Binary, ISO Layer 5 (or 6).
 
## Big Data

Serialization suitble for big data at rest systems, from Hadoop family of solutions.

- [Parquet](https://parquet.apache.org) - Columnar storage for Hadoop workloads. Binary.
- [FlatBuffers](https://google.github.io/flatbuffers/) - Protocol Buffers suitible for larger datasets. Binary.
- [ORC](https://orc.apache.org) - Columnar storage for Hadoop workloads. Binary.
- [Avro](https://avro.apache.org) - Scheme embedded, dynamic rich data structures. Textual/Binary.
- [Ion](https://amzn.github.io/ion-docs/) - Row storage with skip scan parsing. Structed, schema embedded. Amazon. Textual/Binary.

## Scientific

Large scale sparse arrays used in physical, mathematics and statistics research.

- [HDF5®](https://www.hdfgroup.org) - n-dimensional datasets, complex objects, with schema. Efficient I/O. Binary.
- [npy](https://numpy.org/devdocs/reference/generated/numpy.lib.format.html) - Numpy arrays, cell sparse metadata. Binary.

## Machine Learning

Serialization of deep learning networks and weights.

- [SavedModel](https://www.tensorflow.org/guide/saved_model) - TensorFlow package, weights, graph, executable code. Binary.
- [GraphDef](https://www.tensorflow.org/guide/extend/model_files) - TensorFlow graphs. Binary. Deprecated.
- [ONNX](https://onnx.ai) - The open standard for machine learning interoperability
- [safetensors](https://github.com/huggingface/safetensors) - Simple, safe way to store and distribute tensors

## Graph

Serialization formats for representing graph oriented data structures.

- [json-ld](https://json-ld.org) - JSON for Linking Data. Textual.
- [Turtle](https://www.w3.org/TR/turtle/) - Terse RDF Triple Language. Textual.

## Workflow

- [common-workflow-language](https://github.com/common-workflow-language) - Specification for describing analysis workflows and tools in a way that makes them portable and scalable across a variety of software and hardware environments.
- [Relational Algebra and Datalog for Graphs](https://www.coursera.org/lecture/data-manipulation/relational-algebra-and-datalog-for-graphs-U8zVV) - Coursera course on graph data manipulation.

## Language specific

Language native serialization formats for in transit data (aka memory based "live" objects)

### Dart

- [Dart Object Serialization](https://github.com/flutter/packages/tree/main/packages/standard_message_codec) - Ram to Disk serialization. Dart specific. Binary.

### Python

- [pickle](https://docs.python.org/3/library/pickle.html) - Ram to Disk serialization. Binary.
- [msgpack-python](https://github.com/msgpack/msgpack-python) - MessagePack serializer implementation for Python.
- [srsly](https://github.com/explosion/srsly) - Modern high-performance serialization utilities for Python.

### Swift

- [MessagePack.swift](https://github.com/a2/MessagePack.swift) - Swift MessagePack Serializer.

### Java

- [Java Object Serialization](https://docs.oracle.com/javase/8/docs/technotes/guides/serialization/index.html) - Ram to Disk serialization. Binary.


## Academic

Research papers discussing types, category theory, benchamrks and co.

- [Type theory](https://en.wikipedia.org/wiki/Type_theory) - studies types, which informally are attributes that objects can possess.
- [Category theory](https://en.wikipedia.org/wiki/Category_theory) - General theory of functions. Axiomatic foundation for mathematics, as an alternative to set theory.

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Maxim Veksler has waived all copyright and
related or neighboring rights to this work.
