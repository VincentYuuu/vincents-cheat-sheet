ARG RUBY_VERSION
FROM ruby:$RUBY_VERSION-alpine

ARG BUNDLER_VERSION

RUN apk -U add --no-cache \
    build-base \
    git \
    postgresql-dev \
    postgresql-client \
    libxml2-dev \
    libxslt-dev \
    nodejs \
    yarn \
    imagemagick \
    tzdata \
    less \
    && rm -rf /var/cache/apk/*

# COPY .dockerdev/Aptfile /tmp/Aptfile

ENV LANG=C.UTF-8\
    GEM_HOME=/bundle\
    BUNDLE_JOBS=4\
    BUNDLE_RETRY=3\
    RAILS_LOG_TO_STDOUT=true\
    BUNDLE_APP_CONFIG=$GEM_HOME\
    BUNDLE_BIN=$BUNDLE_PATH/bin

ENV PATH /app/bin:$BUNDLE_BIN:$PATH

RUN gem update --system && \
    gem install bundler:$BUNDLER_VERSION

RUN mkdir -p /app

WORKDIR /app

EXPOSE 3000
