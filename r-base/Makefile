LATEST     := $(shell find . -regextype sed -regex ".*/[0-9].*.Dockerfile" | sort -gr | head -n 1)

latest:
	cp -r $(LATEST) latest.Dockerfile
	docker build -t jbgruber/r-base-arm:latest -f latest.Dockerfile .
	export VERSION=`sed -n 's|.*R_VERSION:-\([0-9]\.[0-9]\.[0-9]\).*|\1|p' latest.Dockerfile` && docker tag jbgruber/r-base-arm:latest jbgruber/r-base-arm:"$${VERSION}" && docker push jbgruber/r-base-arm:latest



