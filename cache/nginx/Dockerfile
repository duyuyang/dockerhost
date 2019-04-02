
FROM nginx:1.15-alpine@sha256:816a226b57bb45b6388670b15f1adb60d83240857b2a0d476dd3f0d8d231799d

# Remove origin default config
RUN rm /etc/nginx/conf.d/default.conf
RUN mkdir -p /app/cache/tmp && chown -R nginx /app/cache

COPY config /app/config
COPY run.sh /app/run.sh

CMD ["/app/run.sh"]

VOLUME /app/cache
EXPOSE 80