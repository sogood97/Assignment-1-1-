# 1. base image.
FROM ubuntu:14.04

# 2. Who is the maintainer?
Maintainer LeeKyungSoo "soogood97@khu.ac.kr"

# 3. make directory, echo, 
RUN echo "Made by Kyung Soo"
RUN mkdir /ks417

# 5. Define working directory
WORKDIR /ks417

# 4. Adding files
ADD /line /ks417 


# 6. Where is the portal?
EXPOSE 80

# 7. Check CMD
CMD ["bash"]
