# go_dump1090_exporter_grafana
Grafana dashboard based on the go_dump1090_exporter

This is a multi-container Docker application that is used to scrape the go_dump1090_exporter metrics with Prometheus and then display on a Grafana dashboard. 

### Prerequisites
* Docker
* dump1090-fa

### Setup

1. Clone the repo
```
git clone https://github.com/marvinmartian/go_dump1090_exporter_grafana.git
cd go_dump1090_exporter_grafana
```

2. Move the sample .env file and change the values
```
mv .env.sample .env
```

3. Configure .env with correct IP/path

If you are running on the same host as dump1090-fa, you can volume mount the files directly. Otherwise, you can change the hostname in the .env to your dump1090-fa server.

4. Start-up Containers
```
docker-compose up -d
```

5. Open Grafana in a browser
`http://<ip_address>:3000`

