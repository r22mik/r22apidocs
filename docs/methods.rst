=============
API Methods
=============

Retrieve Inventory
==================


+------------------------+------------------------------------------------------+
| Methods                | Inventory (HTTP METHOD: GET)                         |
+------------------------+------------------------------------------------------+
| Return Type            | JSON string of all inventory                         |
+------------------------+------------------------------------------------------+
| Example                | https://data-service.r22dev.com/partner/inventories  |
+------------------------+------------------------------------------------------+

+--------------+----------+-----------------------------------------------------+
| Parameters   | Required | Notes                                               |
+--------------+----------+-----------------------------------------------------+
| Token        |   YES    | An access token is required for all API requests    |
+--------------+----------+-----------------------------------------------------+
| Pagination   |   NO     | Get specific page                                   |
+--------------+----------+-----------------------------------------------------+
| Page Size    |   NO     | Number of records per page                          |
+--------------+----------+-----------------------------------------------------+

Sample Usage
============

+-----------+------+
| pageSize  | 100  |                   
+-----------+------+
| page      | 3    |
+-----------+------+

Category
========
**Status and Explanation**
     - 1001 : Automotive
     - 1002 : Motorcycles
     - 1013 : Parts
     
Inventory Type
==============
**Status and Explanation**
     - N : New
     - U : Used

API Response (for one unit)
===========================

.. code-block:: python

 "total": 85,
    "totalPage": 5,
    "pageSize": 20,
    "page": 5,
    "inventories": [
        {
            "id": 13091992,
            "created_by": "System",
            "title": "2020 Harley-Davidson Breakout 114",
            "last_mod_by": null,
            "dealer": {
                "id": 101035,
                "dealerName": "Timms Harley Davidson Anderson",
                "active": true,
                "partnerDealerId": null,
                "partnerCode": null,
                "email": null,
                "telephone": null,
                "contact_name": null
            },
            "category": {
                "id": 1002,
                "description": "Motorcycle",
                "titleConvention": "${year} ${make} ${model}",
                "editForm": "dynamic",
                "iconName": "ios-bicycle",
                "iconNameAndroid": "md-bicycle",
                "inventoryCount": null
            },
            "photoCount": 1,
            "status": 1,
            "removed": null,
            "dmsStatus": null,
            "statusChangeCode": "REFRESH",
            "statusChangeNotes": "Refreshed",
            "submissionId": 197554,
            "inventoryDate": null,
            "listingPrice": 21528.00,
            "msrp": null,
            "salePrice": null,
            "wholesalePrice": null,
            "listingComment": null,
            "primaryPhotoUrl": "https://media.r22dev.com/Harley_2020_Jellybeans/20---SOFTAIL---BREAKOUT_114---FXBRS_R.png",
            "detailPageUrl": null,
            "additionalData": null,
            "fields": null,
            "equipments": {},
            "external_id": "1HD1YHK15LB047162",
            "stock_number": "LB047162",
            "inventory_type": "N",
            "details": {
                "make": "Harley-Davidson",
                "year": "2020",
                "model": "Breakout 114",
                "power": "100.00 HP (73.0  kW)) @ 5020 RPM",
                "clutch": "Multi-plate with diaphragm spring in oil bath",
                "torque": "161.36 Nm (16.5 kgf-m or 119.0 ft.lbs) @ 3000 RPM",
                "gearbox": "6-speed",
                "cylinders": "2",
                "rear_tyre": "240/40-R18 ",
                "dry_weight": "294.0 kg (648.2 pounds)",
                "front_tyre": "130/60-B21 ",
                "wheel_base": "1,695 mm (66.7 inches)",
                "bore_stroke": "102.0 x 114.0 mm (4.0 x 4.5 inches)",
                "engine_disp": "1870",
                "final_drive": "Chain, 34/46 ratio primary drive",
                "fuel_system": "Injection. Electronic Sequential Port Fuel Injection",
                "displacement": "1868.00 ccm (113.99 cubic inches)",
                "exhaust_type": "2-into-2 staggered; catalyst in muffler",
                "fuel_control": "Double Overhead Cams/Twin Cam (DOHC)",
                "fuel_capacity": "13.20 litres (3.49 gallons)",
                "odometer_type": "Miles",
                "cooling_system": "Air",
                "engine_details": "V2, four-stroke",
                "overall_length": "2,370 mm (93.3 inches)",
                "exterior_colour": "PERFORMANCE ORG W/PINSTRIPE",
                "rear_suspension": "Twin shocks",
                "front_suspension": "Telescopic fork",
                "odometer_reading": "6"
            },
            "photos": [
                {
                    "id": 390482518,
                    "modifiedDate": "2020-02-19T11:09:59+0000",
                    "originalUrl": "https://media.r22dev.com/Harley_2020_Jellybeans/20---SOFTAIL---BREAKOUT_114---FXBRS_R.png",
                    "photoUrl": "https://media.r22dev.com/Harley_2020_Jellybeans/20---SOFTAIL---BREAKOUT_114---FXBRS_R.png",
                    "thumbnailUrl": "https://media.r22dev.com/Harley_2020_Jellybeans/20---SOFTAIL---BREAKOUT_114---FXBRS_R.png",
                    "photoOrder": 0,
                    "caption": "",
                    "processed": false,
                    "processNote": null
                }
            ]
        }
