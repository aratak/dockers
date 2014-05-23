FROM pandrew/ubuntu-lts
RUN apt-get install -qqy build-essential libssl-dev zlib1g-dev
RUN git clone https://github.com/sstephenson/rbenv.git .rbenv
RUN git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
ENV PATH ~/.rbenv/shims:~/.rbenv/bin:$PATH
RUN echo 'eval "$(rbenv init -)"' >  ~/.bash_profile
RUN rbenv rehash
