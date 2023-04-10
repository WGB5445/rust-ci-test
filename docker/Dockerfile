FROM  rust:1.68.2 as build
WORKDIR /app
COPY . .
RUN arch
RUN cargo build --release

FROM  ubuntu:22.04
COPY --from=build /app/target/release/ci-test /usr/bin


#ENTRYPOINT ["top", "-b"]