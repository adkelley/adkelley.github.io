SITE  = ./site 

clean:
	rm -rf dist
	rm -rf _site

run:
	$(SITE) clean
	$(SITE) build

bp:
	$(SITE) build
	$(SITE) preview


cmp:    
	ghc --make site.hs
	$(SITE) rebuild

bw:
	$(SITE) clean
	$(SITE) build
	$(SITE) watch



########## Mirror to github

deploy: run
	cp -r _site/* ../
