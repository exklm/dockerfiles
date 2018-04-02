> NOTE: It's more like a fork from https://github.com/hut6/docker-postcss.
> However, I prefer to keep all my dockers img in the same place.
> I also changed the Dockerfile to something I can debug easier -> more layers & bigger image.

# docker-postcss

postcss+autoprefixer with Docker. It will also

## Usage

    docker run -it --rm -v $PWD:$PWD -w $PWD exklm/postcss \
		-m \
		-u autoprefixer \
		-u cssnano \
		-o out.min.css \
		original.css

## Build arg
	--build-arg UBUNTU_MIRROR=mirror.0x.sg				// replace with your preferred mirror
	--build-arg VERSION=6.0.11							// postcss version
