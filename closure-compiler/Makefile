all:
	docker build \
		--tag exklm/closure-compiler:latest \
		--build-arg UBUNTU_MIRROR=mirror.0x.sg \
		.
.PHONY: all

push:
	docker push exklm/closure-compiler:latest
.PHONY: push
