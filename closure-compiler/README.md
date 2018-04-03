> NOTE: It's more like a fork from https://github.com/hut6/docker-closure-compiler.
>
> It's probably more inefficient (bigger, more layers), but help me maintain/debug easier.

# exklm/closure-compiler

Google Closure Compiler with Docker

## Usage

```bash
docker run --rm -v $PWD:$PWD -w $PWD closure-compiler \
--js_output_file all.min.js \
--js script1.js script2.js
```
## Build arg

```
--build-arg UBUNTU_MIRROR=mirror.0x.sg				// replace with your preferred mirror
--build-arg VERSION=6.0.11							// postcss version
```
