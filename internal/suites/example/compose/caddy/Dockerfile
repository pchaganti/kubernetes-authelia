FROM caddy:2.8.0-builder AS builder

RUN xcaddy build fix-empty-copy-headers

FROM caddy:2.8.0

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
