# Dockerfile pour l'API
FROM rust:1.82.0 AS dev

WORKDIR /app
COPY . .

# Installer cargo-watch pour surveiller les changements
RUN cargo install cargo-watch

# Commande pour démarrer l'application
CMD ["cargo", "watch", "-x", "run"]
