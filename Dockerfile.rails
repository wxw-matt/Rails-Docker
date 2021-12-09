# alpine3.15 is the minimum version that has libpq-dev
FROM ruby:3.0.3-alpine3.15

RUN set -eux; \
	apk add --no-cache \
		sqlite-dev \
		mariadb-dev \
		libpq-dev \
		ruby-dev \
		make \
		gcc \
		musl-dev \
		build-base \
		tzdata \
		curl \
		nodejs \
		npm \
		yarn \
	;
RUN echo 'gem: --no-document' >> ~/.gemrc
RUN gem install bundler:2.1.4
RUN gem install sassc:2.4.0
RUN gem install listen:3.7.0
RUN gem install selenium-webdriver:4.1.0
# gem "sqlite3", "~> 1.4"
RUN gem install sqlite3:1.4.2
# gem "mysql2", "~> 0.5"
RUN gem install mysql2:0.5.3
# gem "pg", "~> 1.1"
RUN gem install pg:1.2.3
RUN gem install nokogiri:1.12.3
RUN gem install ffi:1.15.3
RUN gem install byebug:11.1.3
RUN gem install rails:6.1.4.1
