FROM library/amazonlinux
WORKDIR /root
ADD scripts root/scripts
RUN yum install -y gcc64-c++ \
libcurl-devel \
cmake3 \
git \ 
nano \
cmake.x86_6 \
gcc-c++.x86_64 \
make.x86_64 \
zip \ 
aws-cli
RUN export CC=gcc64
RUN export CXX=g++64
RUN bash root/scripts/lambda-cpp.sh 

CMD ["/bin/bash"]