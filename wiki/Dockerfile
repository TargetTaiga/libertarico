FROM php:apache

RUN curl -fsSL 'https://releases.wikimedia.org/mediawiki/1.33/mediawiki-1.33.1.tar.gz' -o mediawiki.tar.gz
RUN mkdir wiki
RUN tar xvzf mediawiki.tar.gz --strip-components=1 -C wiki
RUN rm -rf mediawiki.tar.gz
