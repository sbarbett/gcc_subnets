gcc_subnets
======================

A simple client for fetching Google Compute Cloud subnets.

About
======

Google uses DNS TXT records to document the subnets ranges for their cloud platform. For more information see [their FAQ](https://cloud.google.com/compute/docs/faq#where_can_i_find_short_product_name_ip_ranges). This client is designed to automatically query all hostnets containing Google subnets and return them in a simple array.

Installation
=============

```
pip install gcc_subnets
```

Usage
======

```
import gcc_subnets
print gcc_subnets.Client('_cloud-netblocks.googleusercontent.com', '8.8.8.8').get()
```

License
========

This software is made available under the MIT License. For more information, see [here](https://opensource.org/licenses/MIT).