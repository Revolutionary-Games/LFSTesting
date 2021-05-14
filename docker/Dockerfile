FROM fedora:34

RUN dnf install -y --setopt=deltarpm=false ruby git git-lfs && dnf clean all
RUN git lfs install
RUN gem install os colorize

ADD random_script.rb /usr/bin/
RUN chmod +x /usr/bin/random_script.rb
