# hehe

SMART_BAND_SCHEMA = {
  "namespace": "com.example.smart_band",
  "type": "record",
  "name": "SmartBandData",
  "doc": "Dữ liệu sức khỏe từ smart band: vận động, giấc ngủ, sinh tồn và thiết bị.",

  "fields": [
    {"name": "transmission_id", "type": "string",
     "doc": "Mã định danh gói dữ liệu."},
    {"name": "device_id", "type": ["null", "int"], "default": None,
     "doc": "ID thiết bị smart band."},
    {"name": "patient_id", "type": ["null", "string"], "default": None,
     "doc": "Mã bệnh nhân/người dùng."},
    {"name": "created_at", "type": ["null", "long"], "default": None,
     "doc": "Thời điểm ghi nhận (epoch ms)."},
    {"name": "daily_steps", "type": ["null", "int"], "default": None,
     "doc": "Số bước chân trong ngày."},
    {"name": "SpO2", "type": ["null", "int"], "default": None,
     "doc": "Bão hòa oxy trong máu (%)."},
    {"name": "sleep_hours", "type": ["null", "double"], "default": None,
     "doc": "Tổng thời gian ngủ (giờ)."},
    {"name": "deep_sleep_hours", "type": ["null", "double"], "default": None,
     "doc": "Thời gian ngủ sâu (giờ)."},
    {"name": "calories_burned", "type": ["null", "double"], "default": None,
     "doc": "Lượng calo tiêu thụ."},
    {"name": "standing_hours", "type": ["null", "double"], "default": None,
     "doc": "Thời gian đứng/vận động nhẹ."},
    {"name": "run_distance", "type": ["null", "double"], "default": None,
     "doc": "Quãng đường chạy (km)."},
    {"name": "stress_level", "type": ["null", "int"], "default": None,
     "doc": "Mức độ căng thẳng (1–3)."},
    {"name": "heart_rate", "type": ["null", "int"], "default": None,
     "doc": "Nhịp tim trung bình (BPM)."}
  ]
}
