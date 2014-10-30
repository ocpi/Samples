Chargepoints
====

findChargepoints
------------

* `GET /chargepoints` will return all chargepoints
* `GET /chargepoints?nelat=52,2&nelon=5,2&swlat=52,3&swlon=5,3&vehicletype=car&authorizationtype=hubject&authorizationtype=cir` will return all chargepoints matching the search criteria.

```json
[
  {
    "chargepoints":
	  [
	    {
		  "authorization_types": [{"Key":"CIR","Value":"cir"}],
		  "availability":{"description":"","restrictions":"","time":""},
		  "connectors":
		    [
			  {
			    "capabilities":"",
				"charge_protocol":"Mode3",
				"power":{"amperage":16,"current":"AC_3_Phase","voltage":400},
				"price_scheme":
				  {  
				  "display_text":[{"key":"nl-NL","value":"Laadtarieven"}],
				  "expiry_date":"6-11-2014 9:43:44",
				  "price_schema_id":"8e5a884d-c7c3-407b-8d81-0352a7eccc17",
				  "start_date":"21-8-2013 0:00:00",
				  "tariff":
				    [
					  {
					    "condition":"",
						"currency":"EUR",
						"display_text":[{"key":"nl","value":"kWh"},{"key":"en","value":"kWh"}],
						"price_gross":"0.1000",
						"price_net":"0.1200",
						"pricing_unit":"kWhToEV",
						"tariff_id":"xxxxx",
						"tax_pct":21,
						"validity_rule":""
					  },
					  {
					    "condition":"",
						"currency":"EUR",
						"display_text":[{"key":"nl","value":"minuut"},{"key":"en","value":"minute"}],
						"price_gross":"0.0000",
						"price_net":"0.0000",
						"pricing_unit":"charginghours",
						"tariff_id":"xxxxx",
						"tax_pct":21,
						"validity_rule":""
					  },
					]
				  },
				  "status":"Charging",
				  "type":"Onbekend"
				},
			],
			"identifier":"PRO-XXXXXXXX",
			"location":
			  {
			    "chargepoint_location":
				  {
				    "address":"street nr ",
					"city":"City",
					"country":"NL",
					"floor":0,
					"loc":
					  {
					    "lat":xx.xxxxx,
						"lon":x.xxxxx
					  },
					"postal_code":"0000 AA"
				  },
				"entry_location":
				{
				    "address":"street nr ",
					"city":"City",
					"country":"NL",
					"floor":0,
					"loc":
					  {
					    "lat":xx.xxxxx,
						"lon":x.xxxxx
					  },
					"postal_code":"0000 AA"
				},
				"note":"",
				"pictures":null,
				"service_name":"",
				"service_phone":"",
				"service_text":""
			  },
			"name":"PRO-XXXXXXXX",
			"operator":
			  {
			    "description":"",
				"identifier":"PRO",
				"phone":"",
				"url":""
			  },
			"reserved_parking":"2",
			"vehicle_type":"CAR"
		  },
		],
		"num_found":1
	  }
 ]
```

