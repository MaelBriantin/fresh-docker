FROM denoland/deno:2.2.12

WORKDIR /app

COPY ./app .

RUN deno cache deps.ts

EXPOSE 8000

CMD ["deno", "task", "--config", "app/deno.json", "start"]
