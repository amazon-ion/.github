# Amazon Ion

#### [Amazon Ion](https://amazon-ion.github.io/ion-docs/index.html) is a richly-typed, self-describing, hierarchical data serialization format offering interchangeable binary and text representations.
The text format (a superset of JSON) is easy to read and author, supporting rapid prototyping.
The binary representation is efficient to store, transmit, and skip-scan parse.
The rich type system provides unambiguous semantics for long-term preservation of data which can survive multiple generations of software evolution.

Ion was built to address rapid development, decoupling, and efficiency challenges faced every day while engineering large-scale, service-oriented architectures.
It has been addressing these challenges within Amazon for over a decade, and we believe others will benefit as well.

#### [Amazon Ion Hash](https://amazon-ion.github.io/ion-hash/index.html) defines an algorithm for constructing a hash of any Ion value.
For a given Ion value and consistent hash function, the algorithm guarantees hashing the value will always produce the same hash, independent of the value’s encoding (text or binary).
The hash function to use is not declared by the specification—this enables the user to select the hash function most appropriate to their use case.

#### [Amazon Ion Schema](https://amazon-ion.github.io/ion-schema/index.html) defines a grammar and constraints for narrowing the universe of Ion values.
A schema consists of zero or more types, and a type is a collection of zero or more constraints over the Ion data model.
Aspects of a value not constrained by a type (“open content”) are considered valid, which enables loosely-coupled systems to evolve independently.
