# InterSystems IRIS RAG Demo

1. (optional) Edit demo settings in `.env`.
2. (optional, default: SYS) Change IRIS password in `./irispw.txt`.
3. Add your OpenAI key to `./src-iris/openaikey.secret`
4. Build container images: `docker-compose build`.
5. Create containers: `docker-compose up -d`
6. Open IRIS managementportal: http://localhost:8080/csp/sys/UtilHome.csp
7. Open Streamlit: http://localhost:8051/

Additonal commands

- Stop Demo: `docker-compose stop`
- Start Demo: `docker-compose start`
- Delete all docker resources of the demo: `docker-compose down`