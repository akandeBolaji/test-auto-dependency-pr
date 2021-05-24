FROM alpine

RUN apk add --no-cache git go jq nodejs npm && \
    git clone --depth=1 https://github.com/cli/cli.git gh-cli && \
    cd gh-cli

ADD entrypoint.sh /entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]