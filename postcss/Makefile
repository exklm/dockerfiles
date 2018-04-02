all:
	docker build \
		--tag exklm/postcss:latest \
		--build-arg UBUNTU_MIRROR=mirror.0x.sg \
		.
.PHONY: all

push:
	docker push exklm/postcss:latest
.PHONY: push
