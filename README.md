# Depthcharge

<img align="right" src="doc/images/depthcharge-500.png" height="265" width="265">

## What is Depthcharge?

Depthcharge is a toolkit designed to support security research and
"jailbreaking" of embedded platforms using the [U-Boot] bootloader.
It consists of:

* An extensible Python 3 [depthcharge module]
* [Python scripts] built atop of the `depthcharge` module API
* [Depthcharge "Companion" firmware], which is used to perform attacks requiring a malicious peripheral device.
* Some example ["helper" payload binaries] and build scripts to get you started with U-Boot "standalone" program-esque payloads.

[U-Boot]: https://www.denx.de/wiki/U-Boot
[depthcharge module]: ./python/depthcharge
[Python scripts]: ./python/scripts
[Depthcharge "Companion" firmware]: ./firmware/Arduino
["helper" payload binaries]: ./payloads
["standalone"]: https://gitlab.denx.de/u-boot/u-boot/-/blob/v2020.01/doc/README.standalone


## Project Documention

More information can be found in the [online documentation] for the Depthcharge project.

* [Introduction](https://depthcharge.readthedocs.io/en/latest/introduction.html)
  * [What is Depthcharge?](https://depthcharge.readthedocs.io/en/latest/introduction.html#what-is-depthcharge)
  * [Will this be useful for my situation?](https://depthcharge.readthedocs.io/en/latest/introduction.html#will-this-be-useful-for-my-situation)
  * [What are some of its key features?](https://depthcharge.readthedocs.io/en/latest/introduction.html#what-are-some-of-its-key-features)
  * [How do I get started?](https://depthcharge.readthedocs.io/en/latest/introduction.html#how-do-i-get-started)
* [Python Scripts](https://depthcharge.readthedocs.io/en/latest/scripts/index.html)
* [Python API](https://depthcharge.readthedocs.io/en/latest/api/index.html)
* [Companion Firmware](https://depthcharge.readthedocs.io/en/latest/companion_fw.html)
* [Troubleshooting](https://depthcharge.readthedocs.io/en/latest/troubleshooting.html)


If you'd like to build this documentation for offline viewing, You can find the
[Sphinx]-based documentation "source" in the [doc](./doc) directory.

[online documentation]: https://depthcharge.readthedocs.io
[Sphinx]: https://www.sphinx-doc.org/en/master/

## Versioning

Depthcharge uses a [Semantic versioning] scheme for both the Python API and the Companion Firmware.
The version number for published releases will follow that of the Python API version.
The [CHANGELOG](./CHANGELOG) shall document the current version state of both, along
with any compatibility information.

Currently, this project uses ["unstable"] version numbers; API-breaking changes
may occur within this minor version series, if deemed to be sufficiently
beneficial for the future of the project. Refer to the
[CHANGELOG](./CHANGELOG) for guidance on handling any API changes.

Each published release will have a "codename". This serves no real purpose,
other than to amuse the author and add a little fun to preparing releases.
(Maybe they'll even be useful to remember!) The codenames are song titles from
punk bands, increasing alphabetically with each release.

[Semantic versioning]: https://semver.org
["unstable"]: https://semver.org/#spec-item-4

## License

All Depthcharge components are licensed under the [BSD 3-Clause License],
found in the [License.txt] file. Project files use the corresponding
[SPDX Identifier] to denote this.

[BSD 3-Clause License]: https://opensource.org/licenses/BSD-3-Clause
[LICENSE.txt]: ./LICENSE.txt
[SPDX Identifier]: https://spdx.dev/ids
