FROM cuda

RUN yum install -y \
        cuda-samples-$CUDA_PKG_VERSION && \
    rm -rf /var/cache/yum/*

WORKDIR /usr/local/cuda/samples/5_Simulations/nbody
RUN make

CMD ./nbody -benchmark
