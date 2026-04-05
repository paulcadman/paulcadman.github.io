---
title: Lean Portfolio
layout: default
hide_site_title: true
---

# Lean Portfolio

## [lean-ios](https://github.com/paulcadman/lean-ios)

A library to build and run Lean apps in iOS. The project contains:

1. Lean [SDL3](https://wiki.libsdl.org/SDL3/FrontPage) bindings
2. A modified Lean4 source that compatible with iOS
3. Build scripts to build Lean runtime, stdlib and Lean programs for iOS
4. Example applications, including flappy bird

## [lean-effects](https://github.com/paulcadman/lean-effects)

A scoped algebraic effects library for Lean.

## [lens-demo](https://github.com/funexists/lens-demo)

A Lens (composable functional references) library for Lean.

It uses
[metaprogramming](https://github.com/funexists/lens-demo/blob/0c90e83fd65f3b845dc46c1454309e0dbda25a71/Lens/Elab.lean#L13)
to generate the Lens definition boilerplate for a structure.

## [lean-ecs](https://github.com/funexists/lean-ecs)

An entity component system (ECS) library for Lean. An ECS is a common archtectural pattern in video game development.

It uses instance resolution to write functions on entities that have some
combination of components specified in the function type.

It uses
[metapgoramming](https://github.com/funexists/lean-ecs/blob/fbac80e3c0a3bd68361bf779a982e41b3f081603/src/ECS/Elab.lean)
to generate the boilerplate to setup the ECS for user-specified components.

## [raylean](https://github.com/funexists/raylean)

Lean bindings for the [raylib](http://raylib.com) library for video games programming.

### [orbital](https://github.com/funexists/orbital)

A orbital mechanics simulator built using raylean, and lean-ecs.

### [flappy](https://github.com/paulcadman/flappy)

A flappy bird clone in Lean.

## [lean-pan](https://github.com/funexists/lean-pan)

An experiment with using SIMD to accelerate CPU framebuffer rendering in Lean.
