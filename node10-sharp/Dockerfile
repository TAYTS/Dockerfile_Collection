# Use debian as alpine has issues with sharp generate thumbnail (Segmentation fault - core dump)
FROM node:10

WORKDIR /usr/src/app

RUN npm install --save gatsby

# Pre-install dependent libraries needed for gatsby-plugin-sharp to improve build time
RUN npm install --save cwebp-bin@5.1.0
RUN npm install --save mozjpeg@6.0.1
RUN npm install --save pngquant-bin@5.0.2
RUN npm install --save gatsby-plugin-sharp

