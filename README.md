# MathHub News

This repository serves as the source for MathHub News Ticker. 
It is generated using a standard [Jekyll](https://jekyllrb.com) site and can be generated locally using:

    jekyll build

In addition to a normal jekyll output, a file `news.json` is generated. 
This file is automatically placed inside of a docker container, so that the MathHub Frontend has access to it when deployed. 

This is achieved using the automated build [mathhub/news](https://hub.docker.com/r/mathhub/news/) on DockerHub. 
To run it, use

    docker run -p 8043:8043 mathhub/news