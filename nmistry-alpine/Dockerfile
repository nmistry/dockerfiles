FROM alpine:latest
RUN apk add --update wget curl jq htop vim zsh tmux go git && rm -rf /var/cache/apk/*
RUN sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)" || :
ENTRYPOINT ["/bin/zsh"]
