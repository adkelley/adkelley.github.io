SITE  = ./site 

default: install

clean:
	rm -rf dist
	rm -rf _site

build:
	cabal configure
	cabal build

run:
	$(SITE) clean
	$(SITE) build

p:
	$(SITE) watch




########## Mirror to github

deploy: run
	cp -r _site/* ../

