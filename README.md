# snippets

```json
{
	"event_type": "request_mileage",
	"reference": "abcd1234",
	"request" : {
		"vehicle_id" : 1234,
		"target_mileage": 50000
	}
}
```

```json
{
	"event_type": "prediction_mileage",
	"reference": "abcd1234",
	"status": "success",
	"result" : {
		"vehicle_id" : "carabcdefg",
		"target_mileage": 50000,
		"predicted_date": "2018-12-01"
	}
}
```

```json
{
    "event_type": "prediction_mileage",
    "reference": "abcd1234",
    "status": "unpredictable",
    "response": {
        "vehicle_id": 1234,
        "error_code": 100,
        "error_message": "Predicted date is too far in the future to be reliable"
    }
}
```

```json
{
	"event_type": "prediction_mileage",
	"reference": "abcd1234",
	"status": "error",
	"response": {
		"vehicle_id": 1234,
		"error_code": 1,
		"error_message": "No data found for this vehicle ID"
	}
}
```
