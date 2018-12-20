# List of self-hosted image microservices

Trying to find best media micro-service for iXBT.com. 
Can't use commercial CDN like uploadcare/cloudinary because of tight budget. 

Need: 

- Image manipulations (crop, resize, fit, optimize)
- Image proxy from different domains
- Cache proxied/manipulated images

Also:
- Video upload/manipulation
- Easy upload API


### Open source solutions

https://github.com/Pixboost/transformimgs - Open source version of Pixboost transformation. Does not have proxy. 

Only optimize, resize, fit (crop+resize), return as-is for stored files. Written on Go. Compile instructions + Docker image
 -  JPEG + PNG only

https://github.com/spacechop/spacechop - Docker container version of Spacechop. Proxy, Crop, resize, crop (not only center, also right+left!), fit, fill, change format, compress, strip metadata. 
