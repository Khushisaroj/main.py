=== Telemetry Data Transformation Script ===

Loading input data files...

Testing transformation functions...
Testing data-1.json transformation (ISO timestamps)...
Successfully transformed 2 records from format 1
Testing data-2.json transformation (millisecond timestamps)...
Successfully transformed 2 records from format 2

Creating unified output with 2 records
Successfully saved unified data to unified_telemetry_output.json
Testing data transformation functions...

--- Testing Format 1 Transformation ---
Format 1 transformed successfully: 2 records
Sample record: {
  "device_id": "sensor_001",
  "timestamp": 1697380225123,
  "temperature": 23.5,
  "humidity": 65.2,
  "pressure": 1013.25,
  "location": {
    "lat": 40.7128,
    "lon": -74.006
  }
}

--- Testing Format 2 Transformation ---
Format 2 transformed successfully: 2 records
Sample record: {
  "device_id": "sensor_001",
  "timestamp": 1697374225123,
  "temperature": 23.5,
  "humidity": 65.2,
  "pressure": 1013.25,
  "location": {
    "lat": 40.7128,
    "lon": -74.006
  }
}

--- Testing Timestamp Conversion ---
ISO timestamp: 2023-10-15T14:30:25.123Z
Converted to milliseconds: 1697380225123
Converted back to datetime: 2023-10-15T14:30:25.123000Z

--- Comparing with Expected Result ---
✅ SUCCESS: Format 2 transformation matches expected result!

--- Format 1 Transformation Structure Check ---
✅ SUCCESS: Format 1 transformation produces correct structure!
