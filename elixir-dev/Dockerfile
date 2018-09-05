FROM ntenczar/elixir:1.7.2
MAINTAINER Nate Tenczar <ntenczar@gmail.com>

RUN apk --update add bash erlang-crypto erlang-syntax-tools erlang-parsetools \
    erlang-inets erlang-ssl erlang-public-key erlang-eunit \
    erlang-tools erlang-common-test erlang-dev erlang-snmp \
    erlang-runtime-tools erlang-edoc erlang-xmerl \
    erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev wget git && \
    rm -rf /var/cache/apk/*

RUN mix local.hex --force && \
    mix local.rebar --force

CMD ["/bin/bash"]
