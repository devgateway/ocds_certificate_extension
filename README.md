# Certificates

We need a local extension for Direccion Nacional de Vialidad Argentina (DNV) in which we can define specific information about the contracting process such as:

* Certificates

This extension will allow DNV to show more precise information about the certificates been made during the contracting implementation.

## Worked example
The "certificates" extension will be a field inside contracts.implementation, which mean that will be at the same level as transactions

```json
{
  "certificates" : [ 
	{
		"_id" : "0002084/2016",
		"status" : "EMITIDO",
		"date" : "2015-12-01T11:00:00.000Z",
		"certificateAmount" : {
			"amount" : 1000,
			"currency" : "ARS"
		},
		"totalAmount" : {
			"amount" : 2000,
			"currency" : "ARS"
		}
	}, 
	{
		"_id" : "0002447/2016",
		"status" : "PAGADO",
		"date" : "2016-01-01T11:00:00.000Z",
		"certificateAmount" : {
			"amount" : 2000,
			"currency" : "ARS"
		},
		"totalAmount" : {
			"amount" : 8000,
			"currency" : "ARS"
		}
	}
  ]
}

```
