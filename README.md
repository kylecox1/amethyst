<img align="left" width="64px" src="book/src/images/amethyst_thumb.png" />

# Bonsai Simulator


## What is The Bonsai Simulator?

This is an independent project using the Amethyst game engine to create a functioning bonsai tree simulation game. As this is branched from the Amethyst engine
many of the links and documentation will lead back to Amethyst until they are all updated.


## Principles

These principles are what make amethyst unique and competitive in the world of game engines.

* Massively parallel architecture.
* Powered by a correct [Entity Component System][ecs] model.
* Rapid prototyping with [RON][ron] files for prefabs and an abstract scripting API.
* Strong focus on encouraging reusability and clean interfaces.

[ecs]: https://en.wikipedia.org/wiki/Entity–component–system
[ron]: https://github.com/ron-rs/ron

## Why Amethyst?

### Extreme Multithreading

Amethyst is based over a very powerful parallel [ecs] called specs.
This allows games built with Amethyst to maximize the processing power usage to make it run as smooth and as fast as possible, without the headache of multithread programming.

### Clean

By design, the amethyst engine encourages you to write clean and reusable code for your behaviours and data structures, allowing engine users to easily
share useful components, thus reducing development time and cost.

Using the [ecs] architecture, the code of games can be cleanly divided between data and behaviour, making it easy to understand what is going on,
even if the game is running on a massive 64 cores processor.


## Getting started

To compile the current build run:

```
$ cargo run --example bonsai
```

All available examples are listed under [examples][ex].


## Dependencies

If you are compiling on Linux make sure to install the dependencies below.

Additionally, make sure you have EGL installed. Since the package depends on your drivers, we cannot list it here.

### Ubuntu

```
$ sudo apt install libasound2-dev libx11-xcb-dev libssl-dev cmake libfreetype6-dev libexpat1-dev libxcb1-dev
```

### Fedora

```
$ sudo dnf install alsa-lib-devel openssl-devel cmake freetype-devel expat-devel libxcb-devel
```

### Other

See your distribution specific installation process for the equivalent dependencies.

Please note that you need to have a functional graphics driver installed.
If you get a panic about the renderer unable to create the context when trying to run an example,
faulty driver installation can be the issue.

## Contributing

We are a community project that welcomes contributions from anyone.

If you're interested in helping out, please read the [contribution guidelines][cm]
file before getting started.

We have a [good first issue][gfi] category that groups all issues or feature request
that can be made without having an extensive knowledge of rust or amethyst.
Working on those issues is a good, if not the best way to learn.

If you think you are not ready to code yet, you can still contribute by reviewing code written by other members of the community.
In fact, code reviews ensures that the code that gets added to amethyst is of the highest quality as possible.
Pull requests available for reviews are [here][pr].

If for some reason we don't have any open PR or good first issues (that would be a good thing),
you can look through the [issue tracker][it].

[cm]: docs/CONTRIBUTING.md
[pr]: https://github.com/amethyst/amethyst/projects
[it]: https://github.com/amethyst/amethyst/issues
[gfi]: https://github.com/amethyst/amethyst/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22

## License

The Bonsai Simulator is open source software distributed under the terms of both
the [MIT License][lm] and the [Apache License 2.0][la].

[lm]: docs/LICENSE-MIT
[la]: docs/LICENSE-APACHE

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
