> NOTE: It's more like a fork from https://github.com/hut6/docker-postcss.
>
> It's probably more inefficient (bigger, more layers), but help me maintain/debug easier.

# exklm/postcss

postcss+autoprefixer with Docker. It will also

## Usage


```bash
docker run --rm -v $PWD:$PWD -w $PWD exklm/postcss \
	-m \
	-u autoprefixer \
	-u cssnano \
	-o out.min.css \
	original.css
```

## Build arg

```
--build-arg UBUNTU_MIRROR=mirror.0x.sg				// replace with your preferred mirror
--build-arg VERSION=6.0.11							// postcss version
```
