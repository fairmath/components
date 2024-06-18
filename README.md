# FHE components library

This repository is an initial phase of building an application layer FHE Components library for developers and serves as the home to the award-winning solutions from the [FHERMA](https://fherma.io/) challenges platform.
The library will be constantly extended by adding new FHE components.

The initial version of the library contains the results of the first challenges: 
- [Matrix Multiplication](https://fherma.io/challenges/652bf669485c878710fd020b/overview)
- [Logistic Regression Function](https://fherma.io/challenges/652bf648485c878710fd0208/overview)
- [Sign Evaluation](https://fherma.io/challenges/652bf668485c878710fd020a/overview)

 Check out the [FHERMA competition platform](https://fherma.io/) for innovative FHE solutions and challenges.

# FHE backend
Currently, Polycircuit supports two FHE backends:
* OpenFHE
* Lattigo

The library is designed with flexibility in mind, ensuring it's backend-agnostic. 

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/fairmath/components/assets/20524659/374ed5f8-c5c9-4db8-bb38-bb1d8b76dad7">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/fairmath/components/assets/20524659/e72ba649-ecca-46c4-b621-f4b96db1def9">
  <img>
</picture>

# Installation
To use library components, you'll need to install several dependencies and Polycircuit library itself.

## Prerequisites
Ensure you have the following dependencies installed:

* `CMake >= 3.5.1`
* `G++ >= 11.4`
* `Git >= 2.34.1`

## Library installation
To install the header-only Polycircuit library, follow these steps:

1. Clone the repository
```bash
git clone https://github.com/fairmath/polycircuit.git
cd polycircuit
```

2. Configure CMake and install Polycircuit library in /usr/local/include
```bash
cmake .
cmake --build . --target install
```
You can also set a different installation directory:
```bash
cmake . -DCMAKE_INSTALL_PREFIX:PATH=/path/to/include
cmake --build . --target install
```

# Build and run the examples
The examples demonstrate the basic use of a particular component.
To build and run examples, you'll need to install several dependencies.

## Prerequisites
Ensure you have the following dependencies installed:

* `CMake >= 3.5.1`
* `G++ >= 11.4`
* `Git >= 2.34.1`
* `Boost >= 1.74.0`
* `OpenFHE >= 1.1.4`

## Building and running the matrix_mult_usage example:
1. Build:
```bash
cd examples/matrix_mult_usage
cmake -B ./build && make -C ./build -j$(nproc)
```
2. Run (for more info about accepting parameters, see help):
```bash
./build/matrix_mult --help
```

# Contributing to the Library
There are two ways to contribute to Polycircuit:
- Create PR with a new component or improvements for an existing one;
- Participate in the challenges on the [FHERMA platform](https://fherma.io/challenges).

# Stay Connected

Join our vibrant community to stay updated on the latest developments, participate in discussions, and connect with fellow FHE enthusiasts:

* Discord: Join our [Discord server](https://discord.com/invite/NfhXwyr9M5) for real-time chat, Q&A, and community events.
* Twitter: Follow us on [X](https://twitter.com/FairMath) for the latest news, updates, and interesting tidbits from the world of Fully Homomorphic Encryption.
* LinkedIn: Join our [LinkedIn group]() to stay in touch with the team and the updates.
* Visit our [Fair Math blog](https://fairmath.xyz/blog) and [FHERMA challenges wrap-ups](https://fherma.io/content) for in-depth articles, feature announcements, tutorials, and insights into the future of privacy-preserving technologies.
