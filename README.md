# plane_cam  
PX4 SITL için **basit uçak + kamera modeli** (Gazebo Classic).

Bu paket, PX4 simülasyon ortamında kamera entegre edilmiş bir sabit kanatlı uçak modelini hızlıca çalıştırmak ve test etmek için hazırlanmıştır.

---

## Dosya Yapısı

Bu repoda aşağıdaki dosyalar bulunmaktadır:

- **model.config** — Gazebo model yapılandırması  
- **plane_cam.sdf** — Uçağın SDF modeli  
- **plane_cam.sdf.jinja** — PX4 tarafından otomatik oluşturma için Jinja2 şablonu

---

## Hızlı Başlangıç

PX4 SITL ve Gazebo Classic ile çalıştırmak için:

```bash
cd ~/PX4-Autopilot
make px4_sitl gazebo-classic_plane_cam
```
PX4 SITL ve Gazebo Classic ile multi vehicle çalıştırmak için:
```bash
cd /PX4-Autopilot/Tools/simulation/gazebo-classic
./sitl_multiple_run.sh -m plane_cam -n 5
```
