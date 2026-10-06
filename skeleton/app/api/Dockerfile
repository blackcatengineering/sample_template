# Placeholder API image.
# Replace this with the build for the selected API technology.
# Technology: ${{ values.apiTechnology | default('none') }}

FROM alpine:3.20

RUN addgroup -S app && adduser -S app -G app
WORKDIR /app
COPY . /app
USER app
EXPOSE 8080

CMD ["sh", "-c", "echo 'API implementation required'; sleep infinity"]
