FROM mcr.microsoft.com/cbl-mariner/base/nodejs:18.17.1-2-cm2.0.20231004@sha256:4967b4998350f5e438a282c9c40952e182fb744df8d05eae43ff7f62fb267fdf
WORKDIR /app
COPY stats-worker/package*.json ./
RUN npm install
COPY stats-worker/. .

CMD ["npm", "start"]