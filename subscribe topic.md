# การ subscribe topic

1. ไปดู code ใน  

```c
switch ((esp_mqtt_event_id_t)event_id) {
    case MQTT_EVENT_CONNECTED:
....    
```
ซึ่งอยู่ในฟังก์ชันชื่อ 
```
static void mqtt_event_handler(void *handler_args, esp_event_base_t base, int32_t event_id, void *event_data)
```

2. copy บรรทัดต่อไปนี้ลงมาวางไว้ด้านล่าง
```c
        msg_id = esp_mqtt_client_subscribe(client, "KMITL/SIET/65030000/topic/qos1", 1);
        ESP_LOGI(TAG, "sent subscribe successful, msg_id=%d", msg_id);
```
3. แก้ชื่อ topic เป็นตามที่ต้องการ

```c
       // ของเดิม
        msg_id = esp_mqtt_client_subscribe(client, "KMITL/SIET/65030000/topic/qos1", 1);
        ESP_LOGI(TAG, "sent subscribe successful, msg_id=%d", msg_id);

       // ของที่ copy มาวางเพิ่ม
        msg_id = esp_mqtt_client_subscribe(client, "KMITL/SIET/65030000/topic/LED", 1);  // เปลี่ยน .../qos1 เป็น .../LED
        ESP_LOGI(TAG, "sent subscribe successful, msg_id=%d", msg_id);
```
4. โปรแกรมลงบอร์ดแล้วทดสอบโดยการส่ง topic จาก mqtt explorer


