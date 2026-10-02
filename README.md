# visbeat
Code for making anything dance to anything.
Based on "Visual Rhythm and Beat" SIGGRAPH 2018, Abe Davis and Maneesh Agrawala

Project Website: http://abedavis.com/visualbeat/

## Historical learning fork

This repository preserves a learning fork of [Abe Davis's upstream visbeat](https://github.com/abedavis/visbeat), with reading notes added here. The underlying Visual Rhythm and Beat work and software are credited to the upstream authors; this checkout is not presented as an original product or a validated modern runtime.

## Installation provenance

The upstream installation command is `pip install visbeat`. It installs the published package, not this fork's checkout or its reading notes.

The retained [Dockerfile](docker/Dockerfile) creates a Python 2.7 environment, installs the published `visbeat` package, and clones `https://github.com/abedavis/visbeat.git`. Its notebook working directory therefore uses the upstream clone, not this fork. These instructions describe the historical setup; they are not a verified installation guide for this checkout.

## Legacy limits

[setup.py](setup.py) declares Python 2.7 and unpinned dependencies, and the Docker setup also leaves dependency versions unpinned. Installation, examples, media tools, and current platform compatibility remain unverified. Source grammar checks alone do not establish working or safe runtime behavior.

A fresh dependency-resolution audit found advisories in Pillow and youtube-dl. That audit does not establish which versions are installed in an actual legacy Python 2 environment, and no dependency remediation or runtime validation is claimed here.

The upstream [LICENSE](LICENSE) is retained. No new license, redistribution permission, or commercial-use permission is asserted by this fork.
