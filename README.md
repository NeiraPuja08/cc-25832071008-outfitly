# cc-25832071008-outfitly

Cloud Computing — PTI 2802  
Pertemuan 3 — Project Inception

## Author
- **Nama:** [Neira Puja Fazriani]
- **NIM:** [25832071008]
- **Kelas:** [2A]

## Problem
Kebutuhan akan aplikasi web (Outfitly) untuk mengelola koleksi pakaian dan *mix & match*. 
Namun fokus utama pada tahap ini adalah deployment aplikasi web Flask ke infrastruktur VPS Ubuntu Server 24.04 menggunakan Gunicorn, systemd, dan reverse proxy Caddy.

## Target Users
- Pengguna personal, seperti mahasiswa dan pekerja, yang ingin mengelola koleksi pakaian serta membuat kombinasi outfit (Mix & Match) secara mandiri.
- Dosen pengampu Mata Kuliah Cloud Computing (PTI 2802) sebagai penilai proyek.

## Features M03
- baseline application (`/`)
- health check endpoint (`/health`)
- VPS deployment dengan Caddy & systemd

## Architecture

```mermaid
flowchart LR
    U[User] --> C[Caddy]
    C --> G[Gunicorn]
    G --> F[Flask]

