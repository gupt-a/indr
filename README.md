# indr
Yet another C++ library for using the Discord API

## Installing
This library is currently under development, wait for an actual release before trying to install it.

## Examples
TODO

The full documentation is available [here](blah).

## Requirement
For now I only wrote this with Linux servers in mind so if you want to run this on a Linux server
just make sure you have Boost and OpenSSL installed, then build this with CMake. All other third-party
code is included in this repository itself so you don't need to install anything else.


## Supported platforms and compilers
While I have tried my best to use cross-platform code wherever possible, indr is still very, very alpha.
I haven't even tried to compile it on a different system yet. So yeah, getting it work on other platforms is far in the 
future. It seems to work pretty well on the stable Debian release with GCC 7.5.0, though.

## TODO
This is just a list of things I plan to work on, don't pay too much attention to it.
  * Do actual tests, check for memory leaks with Valgrind, and other stuff to make the lib more stable and production-ready.
  * Optimize, optimize, optimize...gotta be fast otherwise using C++ makes little sense. (unless of course, if you just HATE javascript)
  * Support for ETF payloads in gateway.
  * Have full voice capability, with support for popular audio formats. (*cough* FFMPEG *cough*)
  * use async logging with spdlog

## License
indr is licensed under the MIT license. See the [license file](LICENSE).

indr uses some third-party code and separate licenses may be applicable to it, it's all there
in one place in [this folder](include/third_party).