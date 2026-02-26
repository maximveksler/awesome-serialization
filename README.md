# awesome-serialization [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> So many formats, so much wow. *See [wesm](https://github.com/18F/data-act-pilot/issues/161#issuecomment-139812420) comment before making up your mind.*

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
- [Streaming](#streaming)
- [Security-Focused](#security-focused)
- [Configuration](#configuration)
- [Academic](#academic)

### **API**

Serialization suitable for API RPC networked services.

- [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) - Comma Separated Values. Textual.
- [JSON](https://www.json.org) - Lightweight document data-interchange format. Textual.
- [JSONL](https://jsonlines.org) - Schemeless "multiple JSON documents in 1 file" container data format. Textual.
- [JSON5](https://json5.org/) - JSON with added support for comments and relaxed syntax. Textual.
- [Thrift](http://thrift.apache.org) - Scalable code generation, schema evolution binary format. Binary.
- [Protocol Buffers](https://github.com/protocolbuffers/protobuf) - Google's data interchange format. Binary.
- [Message Pack](https://msgpack.org) - Efficient JSON-like binary serialization format. Binary.
- [bson](http://bsonspec.org) - Binary schemeless JSON encoding. Binary.
- [XML](https://www.w3.org/XML/) - Extensible Markup Language. Genuinely Horrible. Textual.
- [Plist](https://en.wikipedia.org/wiki/Property_list) - Property List representation. Apple. Textual.
- [YAML](https://yaml.org) - Indentation-based data serialization standard. Textual.
- [TOML](https://github.com/toml-lang/toml) - Tom's Obvious, Minimal Language. Textual.
- [CBOR](https://cbor.io) - Concise Binary Object Representation. Schema-free. Binary.
- [ION](https://amzn.github.io/ion-docs/) - Amazon's advanced JSON-compatible serialization. Textual/Binary.
- [Smile](https://github.com/FasterXML/smile-format-specification) - Binary JSON format from FasterXML/Jackson. Used in Elasticsearch. Binary.

### **RPC**

- [gRPC](https://grpc.io) - A high-performance, open source universal RPC framework. Binary, ISO Layer 7.
- [RSocket](https://rsocket.io) - Application protocol providing Reactive Streams semantics. Binary, ISO Layer 5 (or 6).
- [Cap’n Proto](https://capnproto.org/) - High-performance, schema-based data interchange format. Binary.
- [FlatBuffers](https://google.github.io/flatbuffers/) - Suitable for zero-copy deserialization. Binary.
- [Connect](https://connectrpc.com/) - Modern RPC framework compatible with gRPC, with HTTP/1.1, JSON, and browser support. Binary/Textual.

### **Big Data**

Serialization suitable for big data at rest systems, from Hadoop family of solutions.

- [Parquet](https://parquet.apache.org) - Columnar storage for Hadoop workloads. Binary.
- [FlatBuffers](https://google.github.io/flatbuffers/) - Protocol Buffers suitable for larger datasets. Binary.
- [ORC](https://orc.apache.org) - Columnar storage for Hadoop workloads. Binary.
- [Avro](https://avro.apache.org) - Scheme embedded, dynamic rich data structures. Textual/Binary.
- [Ion](https://amzn.github.io/ion-docs/) - Row storage with skip scan parsing. Structured, schema embedded. Amazon. Textual/Binary.
- [Arrow](https://arrow.apache.org) - Cross-language columnar data format optimized for analytics workloads. Binary.
- [Delta Lake](https://delta.io/) - Transactional storage layer for big data workflows. Binary.
- [Iceberg](https://iceberg.apache.org/) - Open table format for large datasets. Binary.
- [Lance](https://lancedb.github.io/lance/) - Modern columnar format optimized for ML and vector search workloads. Binary.

### **Scientific**

Large-scale sparse arrays used in physical, mathematics, and statistics research.

- [HDF5®](https://www.hdfgroup.org) - n-dimensional datasets, complex objects, with schema. Efficient I/O. Binary.
- [npy](https://numpy.org/devdocs/reference/generated/numpy.lib.format.html) - Numpy arrays, cell sparse metadata. Binary.
- [NetCDF](https://www.unidata.ucar.edu/software/netcdf/) - Self-describing, machine-independent data format for scientific data. Binary.
- [Zarr](https://zarr.readthedocs.io/) - Scalable storage of n-dimensional arrays. Binary.
- [ASDF](https://asdf-standard.readthedocs.io/) - Advanced Scientific Data Format for astronomy and beyond. Binary/Textual.

### **Machine Learning**

Serialization of deep learning networks and weights.

- [SavedModel](https://www.tensorflow.org/guide/saved_model) - TensorFlow package, weights, graph, executable code. Binary.
- [CoreML](https://developer.apple.com/documentation/coreml) - Apple's on-device ML model format. Binary.
- [ONNX](https://onnx.ai) - Open Neural Network Exchange. Interoperability focused. Binary.
- [MLIR](https://mlir.llvm.org/) - Intermediate representation for machine learning computations. Textual/Binary.
- [TorchScript](https://pytorch.org/docs/stable/jit.html) - Serialization for PyTorch models. Binary.
- [GGUF](https://github.com/ggerganov/ggml/blob/master/docs/gguf.md) - Quantized model format for llama.cpp/ggml. The de facto standard for local LLM inference. Binary.
- [MLX format](https://ml-explore.github.io/mlx/) - Apple's ML framework format, safetensors-based. Optimized for Apple Silicon. Binary.

<!-- trunk-ignore(markdownlint/MD001) -->
###### Deprecated in Machine Learning

- [GraphDef](https://www.tensorflow.org/guide/extend/model_files) - TensorFlow graphs. Binary.
- [PMML](https://dmg.org/pmml/v4-4/GeneralStructure.html) - Predictive Model Markup Language for exchanging ML models.

### **Graph**

Serialization formats for representing graph-oriented data structures.

- [json-ld](https://json-ld.org) - JSON for Linking Data. Textual.
- [Turtle](https://www.w3.org/TR/turtle/) - Terse RDF Triple Language. Textual.
- [GraphML](http://graphml.graphdrawing.org/) - XML-based graph serialization format. Textual.
- [DOT](https://www.graphviz.org/doc/info/lang.html) - Graph description language, developed as a part of the Graphviz project. Textual.
- [ParquetGraph](https://github.com/graphfoundry/parquet-graph) - Integration of Parquet with graph data structures. Binary.
- [GraphSON](https://tinkerpop.apache.org/docs/current/dev/io/#graphson) - JSON-based graph serialization. Textual.

<!-- trunk-ignore(markdownlint/MD001) -->
###### Deprecated in Graph

- [GraphML](http://graphml.graphdrawing.org/) - XML-based graph serialization format. Textual.- [GML](https://en.wikipedia.org/wiki/Graph_Modelling_Language) - Graph Modeling Language. Hierarchical ASCII-based. Textual.

### **Workflow**

- [common-workflow-language](https://github.com/common-workflow-language) - Specification for describing analysis workflows and tools in a way that makes them portable and scalable across a variety of software and hardware environments.
- [Apache Airflow DAGs](https://airflow.apache.org) - Python-based Directed Acyclic Graphs for workflows.
- [WDL](https://openwdl.org/) - Workflow Description Language for genomics and scientific workflows.
- [Relational Algebra and Datalog for Graphs](https://www.coursera.org/lecture/data-manipulation/relational-algebra-and-datalog-for-graphs-U8zVV) - Coursera course on graph data manipulation.
- [Cromwell](https://cromwell.readthedocs.io/) - Scientific workflow management, compatible with WDL and CWL.
- [Nextflow](https://www.nextflow.io/) - Scalable and reproducible scientific workflows.

### **Programming**

Language-native serialization formats for in-transit data (aka memory-based "live" objects).

#### **JavaScript**

- [BSON.js](https://github.com/mongodb/js-bson) - BSON serializer. Binary.
- [avsc](https://github.com/mtth/avsc) - JavaScript implementation of Apache Avro. Textual.

#### **Dart**

- [Dart Object Serialization](https://github.com/flutter/packages/tree/main/packages/standard_message_codec) - RAM to Disk serialization. Dart-specific. Binary.

#### **Python**

- [pickle](https://docs.python.org/3/library/pickle.html) - RAM to Disk serialization. Binary.
- [msgpack-python](https://github.com/msgpack/msgpack-python) - MessagePack serializer implementation for Python.
- [srsly](https://github.com/explosion/srsly) - Modern high-performance serialization utilities for Python.

#### **Swift**

- [MessagePack.swift](https://github.com/a2/MessagePack.swift) - Swift MessagePack Serializer.

#### **Java**

- [Java Object Serialization](https://docs.oracle.com/javase/8/docs/technotes/guides/serialization/index.html) - RAM to Disk serialization. Binary.

#### **Rust**

- [Serde](https://serde.rs/) - Rust's serialization framework for multiple formats like JSON, CBOR, and MessagePack.
- [bincode](https://github.com/bincode-org/bincode) - High-performance binary serialization for Rust.

#### **Go**

- [GOB](https://pkg.go.dev/encoding/gob) - Go's built-in serialization format for arbitrary data structures. Binary.

### **Streaming**

Serialization formats optimized for real-time streaming data.

- [Protobuf-Lite](https://github.com/protocolbuffers/protobuf-javalite) - Lightweight Protocol Buffers for constrained environments.
- [CloudEvents](https://cloudevents.io/) - CNCF specification for describing event data in a common way. Textual/Binary.
- [AsyncAPI](https://www.asyncapi.com/) - OpenAPI equivalent for event-driven and message-driven architectures. Textual.

### **Security-Focused**

Serialization formats designed with security and robustness in mind.

- [safetensors](https://github.com/huggingface/safetensors) - Safe serialization of tensors for machine learning. Binary.
- [Sealed Object Serialization](https://developer.mozilla.org/en-US/docs/Web/API/SubtleCrypto/encrypt) - Encrypted serialization for web data. Textual/Binary.
- [PASETO](https://paseto.io/) - Platform-Agnostic Security Tokens. Secure alternative to JWT. Textual.
- [COSE](https://datatracker.ietf.org/doc/html/rfc8152) - CBOR Object Signing and Encryption. Used in WebAuthn/FIDO2. Binary.

### **Configuration**

Serialization formats designed for application and infrastructure configuration.

- [CUE](https://cuelang.org/) - Constraint-based configuration language with validation, templating, and JSON superset. Google. Textual.
- [Pkl](https://pkl-lang.org/) - Programmable, typed configuration language. Apple. Textual.
- [KCL](https://kcl-lang.io/) - Kusion Configuration Language for cloud-native config and policy. Textual.

### **Academic**

Research papers discussing types, category theory, benchmarks & co.

- [Type theory](https://en.wikipedia.org/wiki/Type_theory) - Studies types, which informally are attributes that objects can possess.
- [Category theory](https://en.wikipedia.org/wiki/Category_theory) - General theory of functions. Axiomatic foundation for mathematics, as an alternative to set theory.
- [Graph Compression Techniques](https://arxiv.org/abs/2006.03684) - Research on optimizing graph serialization.
- [Efficient Serialization in Distributed Systems](https://arxiv.org/abs/2201.02357) - Study of efficient serialization techniques for scalability.

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Maxim Veksler has waived all copyright and
related or neighboring rights to this work.
