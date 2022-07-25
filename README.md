# envoy-actions ![Lincense](https://img.shields.io/github/license/oslook/envoy-actions)

## Getting Started

## Requirements
  - System: MacOS, Ubuntu or Windows
  - Bazel
  - Docker

## Installation

## Build and run Examples by Github Actions

### :dart: Envoy

- build in docker ( Windows，Ubuntu )
[![Envoy(Ubuntu Docker Image)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-in-docker.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-in-docker.yml)


- build with bazel (MacOS, Windows, Ubuntu)
[![Envoy(Local Ubuntu)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-ubuntu.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-ubuntu.yml)


- build in sandbox
[![Envoy(Ubuntu Docker sandbox)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-in-sandbox.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/envoy-in-sandbox.yml)

  - supported：ubuntu  
  - :whale: build on docker image like `envoyproxy/envoy-build-ubuntu`  

### :dart: envoy-mobile

 Mobile client networking libraries based on the Envoy project.

To build Envoy Mobile, your system must also be set up for building Envoy. To get started, you can use the Github Action Workflows.

Envoy Mobile can build on MacOS, selected macOS for the 3 cpu cores. 

The output of Envoy Mobile for each launguage(Android，iOS):
  - Java: envoy_android_aar_sources
  - Kotlin: envoy_android_aar_sources
  - objective-c: envoy_ios_framework
  - Swift: envoy_ios_cocoapods

Github Action Workflows
- Android 
[![envoy-mobile-android-build](https://github.com/oslook/envoy-actions/actions/workflows/mobile-android-build.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/mobile-android-build.yml)

  - CPU Arch supported: `x86, armeabi-v7a, arm64-v8a`  (Official only `x86`)  

- iOS 
[![envoy-mobile-ios-build](https://github.com/oslook/envoy-actions/actions/workflows/mobile-ios-build.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/mobile-ios-build.yml)
  - CPU Arch supported:	i386,x86_64,armv7,arm64  


- Artifacts
[![envoy-mobile-artifacts](https://github.com/oslook/envoy-actions/actions/workflows/mobile-artifacts.yml/badge.svg)](https://github.com/oslook/envoy-actions/actions/workflows/mobile-artifacts.yml)
  - The workflow not use the github cache, fully build and upload the sdk and examples.

### :dart:	envoy-mobile-app

TODO:

## Compatible Envoy builds

Envoy is the first host side implementation of Proxy-Wasm ABI, 
and we run end-to-end tests with multiple versions of Envoy and Envoy-based [istio/proxy](https://github.com/istio/proxy) in order to verify each Proxy-Wasm SDK works as expected.

Please refer to [workflows](.github/workflows) for which version is used for End-to-End tests.


## External links

- [WebAssembly for Proxies (ABI specification)](https://github.com/proxy-wasm/spec)
- [WebAssembly for Proxies (AssemblyScript SDK)](https://github.com/solo-io/proxy-runtime)
- [WebAssembly for Proxies (C++ SDK)](https://github.com/proxy-wasm/proxy-wasm-cpp-sdk)
- [WebAssembly for Proxies (Rust SDK)](https://github.com/proxy-wasm/proxy-wasm-rust-sdk)
- [WebAssembly for Proxies (Zig SDK)](https://github.com/mathetake/proxy-wasm-zig-sdk)
