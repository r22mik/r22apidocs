=============
API Endpoints
=============

+------------------------+------------------------------------------------------+
| Production Environment | https://data-service.r22dev.com/partner/inventories  |
+------------------------+------------------------------------------------------+
| URL Parameters         | @RequestParam(required = false) Integer page,        |
|                        | @RequestParam(required = false) Integer pageSize     |
+------------------------+------------------------------------------------------+
| URL Example            | http://data-service.r22dev.com/partner/inventories?  |
|                        | pageSize=150&page=2                                  |
+------------------------+------------------------------------------------------+
.. note:: The default page size is 50

cURL
====
curl --location --request GET
'http://data-service.r22dev.com/partner/inventories?pageSize=20&page=5' \
--header 'Authorization: Bearer {Input your token here}
