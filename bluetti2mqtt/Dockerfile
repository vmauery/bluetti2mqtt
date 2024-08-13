ARG BUILD_FROM
FROM $BUILD_FROM

# Copy data for add-on
COPY rootfs /

# Install bluetti_mqtt
RUN apk add --update --no-cache bluez git
RUN pip install git+https://github.com/ftrueck/bluetti_mqtt
run apk del git \
	&& rm -rf /var/cache/apk/* /lib/apk/db/*

CMD [ "/run.sh" ]
