---
title: Lean Portfolio
layout: default
hide_site_title: true
---

# Lean Portfolio

This page gives an overview of some of my Lean projects.

## [lean-ios](https://github.com/paulcadman/lean-ios)

A framework for building and running Lean applications on iOS simulators and devices.

It includes:

1. A modified `lean4` source repository that's compatible with the iOS toolchain
2. Build scripts for the Lean runtime, stdlib, and Lean programs for iOS
3. Lean [SDL3](https://wiki.libsdl.org/SDL3/FrontPage) FFI bindings
4. Example applications, including a Flappy Bird game

## [lean-effects](https://github.com/paulcadman/lean-effects)

A scoped algebraic effects library for Lean. The implementation is based on an
[Agda library](https://github.com/JonasHoefer/scoped-effects-agda) by Jonas
Höfer. One of the main challenges in the implementation was how to define the
[Prog](https://github.com/paulcadman/lean-effects/blob/1b9b70091d685e90be5033fa07b3892e3e4159e4/Effects/Prog.lean#L49)
type. In order for Lean to accept the doubly-nested inductive type (needed to
define scoped effect handlers), a nested induction is required.

## [lens-demo](https://github.com/funexists/lens-demo)

A demo lens library for Lean. Lenses are composable functional references for
immutable data access and update.

It uses
[metaprogramming](https://github.com/funexists/lens-demo/blob/0c90e83fd65f3b845dc46c1454309e0dbda25a71/Lens/Elab.lean#L13)
to generate the lens definition boilerplate for a structure automatically.

## [lean-ecs](https://github.com/funexists/lean-ecs)

An entity component system (ECS) library for Lean. ECS is a common architectural
pattern in game development.

Users can write functions over particular combinations of components and these
are translated to entity updates via instance resolution.

It uses
[metaprogramming](https://github.com/funexists/lean-ecs/blob/fbac80e3c0a3bd68361bf779a982e41b3f081603/src/ECS/Elab.lean)
to generate the boilerplate needed to set up the ECS for user-specified components.

## [raylean](https://github.com/funexists/raylean)

Lean bindings for the [raylib](http://raylib.com) library for graphics and game programming.

### [orbital](https://github.com/funexists/orbital)

An orbital mechanics simulator built using raylean and lean-ecs.

### [flappy](https://github.com/paulcadman/flappy)

A Flappy Bird game written built using raylean.

## [lean-pan](https://github.com/funexists/lean-pan)

An experiment in using SIMD to accelerate CPU framebuffer rendering in Lean.
