FROM --platform=linux/arm64 rust:1.68.2
WORKDIR /app
COPY . .
RUN cargo build --release

#ENTRYPOINT ["top", "-b"]