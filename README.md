# InterSystems IRIS RAG Demo

1. (optional) Edit demo settings in `.env`.
2. (optional, default: SYS) Change IRIS password in `./irispw.txt`.
3. Add your OpenAI key to `./src-iris/openaikey.secret`
4. Build container images: `docker-compose build`.
5. Create containers: `docker-compose up -d`
6. Open IRIS managementportal: http://localhost:8080/csp/sys/UtilHome.csp
7. Open Streamlit: http://localhost:8051/

# To Demo:
(Without RAG)
1. On Chat Inferface, type "when is the Singapore Fintech Festival held?"
2. Notice the output giving a generic response of it being usually held in November each year

(With RAG)
1. In Management Portal, Enable the  `Start PDF Import Local`. This imports 2 PDFs, one on the background of a Logystics company, and the other on the SFF 2024 Agenda.
2. Return to the Chat Interface, enter in the same question as above
3. Notice the output being more specific that the event is held on 6-8 Nov.
4. Head to the Visual Trace, locate the 
