FROM tsuru/base-platform

ADD	. /var/lib/tsuru/java
RUN	sudo cp /var/lib/tsuru/base/deploy /var/lib/tsuru

RUN set -ex; \
    sudo /var/lib/tsuru/java/install; \
    sudo rm -rf /var/lib/apt/lists/*

# RUN set -x \
#     && echo "sdkman_auto_answer=true" > $SDKMAN_DIR/etc/config \
#     && echo "sdkman_auto_selfupdate=false" >> $SDKMAN_DIR/etc/config \
#     && echo "sdkman_insecure_ssl=false" >> $SDKMAN_DIR/etc/config