# tugas-sesi-3
REST API dengan FastAPI
from fastapi import FastAPI

# Inisialisasi aplikasi FastAPI
app = FastAPI(title="API Rekomendasi & Transportasi")

# Endpoint 1: Rekomendasi Tempat Wisata
@app.get("/api/v1/recommendations")
def get_recommendations():
    return ["Tokyo Tower", "Mount Fuji", "Shibuya"]

# Endpoint 2: Pilihan Moda Transportasi
@app.get("/api/v1/transportations")
def get_transportations():
    return ["Bus", "Train", "Flight"]
