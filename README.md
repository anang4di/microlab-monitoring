
# Microlab Monitoring

Sistem pemantauan berbasis Prometheus dan Grafana sederhana, dirancang untuk memberikan visibilitas real-time terhadap parameter lingkungan dan performa server.

## Feaures

- **Integrasi Prometheus**: Mengumpulkan metrik dari berbagai sumber (ex: node exporter).
- **Visualisasi dengan Grafana**: Dashboard untuk memantau data secara real-time.
- **Docker-Compose**: Kemudahan dalam manajemen layanan.

## Technology

- **Prometheus**: Sistem monitoring dan alerting open-source.
- **Grafana**: Platform analitik dan visualisasi data.
- **Docker**: Platform untuk mengembangkan, mengirim, dan menjalankan aplikasi dalam kontainer.
- **Docker-Compose**: Tool untuk mendefinisikan dan menjalankan aplikasi multi-kontainer Docker.

## Project Structure
```
microlab-monitoring/
├── docker-compose.yml
├── prometheus/
│   └── prometheus.yml
└── grafana/
    └── data/
```

## How to Use

1. **Clone Repository**
	```bash
	git clone https://github.com/anang4di/microlab-monitoring.git
	cd microlab-monitoring
	```
2. **Jalankan dengan Docker Compose**
	```bash
	docker-compose up -d
	```
3. **Sesuaikan konfigurasi Prometheus**

	Edit `prometheus.yml` sesuaikan target server yang akan dimonitor.
	
5. **Akses Dashboard Grafana**
	-   Buka browser dan navigasi ke `http://localhost:3000`
    -   Login dengan:
        -   **Username**: `admin`
        -   **Password**: `admin`
    -   Import dashboard yang tersedia atau buat dashboard baru sesuai kebutuhan.
