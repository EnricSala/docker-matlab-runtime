# docker-matlab-runtime
Docker image containing the Matlab Compiler Runtime, based on `java:8-jre`.

### Instructions

1. Go to the desired version directory:

       cd R2015b

2. Download the corresponding runtime from: [MATLAB Runtime](https://www.mathworks.com/products/compiler/mcr.html)

       wget https://...... -O MCR_R2015b.zip

3. Build the image:

       docker build -t mcr:R2015b .

4. Use the image in other dockerfiles:

       FROM mcr:R2015b
       ...
