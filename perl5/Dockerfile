FROM perl:latest

ADD . /opt/adventure/perl5
WORKDIR /opt/adventure/perl5

# TODO use cpanfile instead?
RUN cpanm Moo
RUN cpanm YAML

# TODO are we making an assumption about the mission?
CMD [ "perl", "-Ilib", "actioncastle.pl" ]
