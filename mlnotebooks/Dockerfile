FROM sampathkethineedi/base-notebook:0.1

COPY ZscalerRootCertificate-2048-SHA256.crt /cert/

# install additional package...
RUN pip install --no-cache-dir nbgitpuller --cert /cert/ZscalerRootCertificate-2048-SHA256.crt && \
    jupyter serverextension enable --py nbgitpuller --sys-prefix
