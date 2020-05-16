latest:
	docker build -t jbgruber/rstudio-arm:latest -f latest.Dockerfile .
	export VERSION=`cat latest.Dockerfile | head -n1 | sed 's/.*\([0-9].[0-9].[0-9]\)/\1/'` && docker tag jbgruber/rstudio-arm jbgruber/rstudio-arm:"$$VERSION"
	

