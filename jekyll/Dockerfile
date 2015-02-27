FROM dock0/arch
MAINTAINER Matt Everson "mattreverson@gmail.com"

RUN pacman -Sy --needed --noconfirm make gcc sed patch ruby nodejs python2 python-pygments && pacman -Scc --noconfirm
RUN gem install github-pages --no-ri --no-rdoc --no-user-install

EXPOSE 4000
VOLUME ["/source"]
WORKDIR /source
ENTRYPOINT ["jekyll"]

