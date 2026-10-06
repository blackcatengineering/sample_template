# Placeholder web image.
# Replace this with the build for the selected web technology.
# Technology: ${{ values.webTechnology | default('none') }}
# Server: ${{ values.webContainer | default('none') }}

FROM nginx:alpine

COPY . /usr/share/nginx/html

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]
