# COLABRIQ Decentralized Knowledge Graph

## Introduction

This is the open source reference edition of COLABRIQ's Decentralized Knowledge Graph and information sharing protocol. This component is a parent project that allows you to build and run the whole system. Please agree to [LICENSE.md](LICENSE.md) and read [CONTRIBUTING.md](CONTRIBUTING.md) before using this code.

## How to run

 1. Check this module out and initialize git the submodules.
 2. Run `mvn install` at the top level to install any SNAPSHOT version dependencies into your local repository
 3. Run `mvn dependency:copy-dependencies` to prepare to run each module.

See below for instructions on running each module.

It is also possible to use the `Dockerfile` files found in the repositories.
These need to be updated and further instructions will be available soon.

### Running the DHT engine

The following command runs the DHT engine:

`java -jar sccp-rdf/target/rdfendpoint-0.2-SNAPSHOT.jar <configFile>`

You will need a config file as the first argument.
A number of samples config files are located at `sccp-tests/src/test/resources/`.

### Running the RDF endpoint 

The following command runs the RDF endpoint:

`java -jar sccp-rdf/target/rdfendpoint-0.2-SNAPSHOT.jar <configFile>`
  
You will need a config file as the first argument.
A number of samples config files are located at `sccp-tests/src/test/resources/`.

## How to develop

See instructions in [CONTRIBUTING.md](CONTRIBUTING.md).

After running `mvn install` you should be able to import `sccp-parent` as Maven parent project, with its children, in to Eclipse or IntelliJ.

