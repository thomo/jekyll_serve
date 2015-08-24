# jekyll_serve
A docker image (based on CentOS 7) with jekyll (http://jekyllrb.com/)

# Usage
Run on command line

## Generate new jekyll site project
To generate a new site 

    docker run --rm -i -t -v $(pwd)://data -p 4000:4000 thomo/jekyll new my_famous_site

## Build and View site

	cd my_famous_site
    docker run --rm -i -t -v $(pwd)://data -p 4000:4000 thomo/jekyll 

Than visit the jekyll output on http://<docker ip>:4000 

## Edit site content
Just edit the content in _post ...