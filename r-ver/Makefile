
latest: 
	docker build -t jbgruber/r-ver-arm:latest -f latest.Dockerfile .
	export VERSION=`sed -n 's|.*R_VERSION:-\([0-9]\.[0-9]\.[0-9]\).*|\1|p' latest.Dockerfile` && docker tag jbgruber/r-ver-arm:latest jbgruber/r-ver-arm:"$${VERSION}" && docker push jbgruber/r-ver-arm:latest



