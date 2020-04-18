# Assignment.1
For data center programming assignment #1
<7>


부족하지만 도커 파일을 스스로 만들어 보아야 도커파일을 제대로 이해할 수 있다고 생각해서,
reading article을 많이 참조해 스스로 만들어 보았습니다.


# 1. base image.
FROM ubuntu:14.04

-> 먼저 도커 이미지를 가져옵니다. 


# 2. Who is the maintainer?
Maintainer LeeKyungSoo "soogood97@khu.ac.kr"

-> maintainer를 표시하는 자리이며, 저는 교수님이 하던 방식으로 만들었습니다.


# 3. make directory, echo.
RUN echo "Made by Kyung Soo"
RUN mkdir /ks417

-> RUN으로 실행한 결고가 이미지위에 저장이 되며, 저는 "Made by Kyung Soo"를 이미지를 불러오는 과정에서 표시하도록 설정했습니다.
   또한 ubuntu가 실행 될 directory를 새로 만들어 보았습니다. 


# 4. Define working directory
WORKDIR /ks417

-> Work directory를 ks417로 지정해, 컨테이너를 실행하면 바로 들어갈 수 있도록 했습니다.


# 5. Adding files
ADD /line /ks417 

-> line은 도커파일이 존재하는 컨텍스트 하부에 존재하는 폴더 이름입니다. 
   저는 이 폴더에서(비록 아무것도 넣지 않았지만) ks417로 복사한다는 가정을 세워보았습니다.


# 6. Check CMD
CMD ["bash"]

-> 명령은 기본에서 크게 다르게는 만들지 않았습니다.



여기까지 입니다. 감사합니다!!
