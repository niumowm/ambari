<!---
Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements. See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to You under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

List Services
=====

[Back to Resources](index.md#resources)

Returns a collection of the services in a given cluster.

    GET /clusters/:name/services

**Response**

    200 OK
    {
    	"href" : "http://your.ambari.server/api/v1/clusters/c1/services",
    	"items" : [
    		{
        		"href" : "http://your.ambari.server/api/v1/clusters/c1/services/NAGIOS",
        		"ServiceInfo" : {
          			"cluster_name" : "c1",
          			"service_name" : "NAGIOS"
          		}
        	},
        	{
        		"href" : "http://your.ambari.server/api/v1/clusters/c1/services/HCATALOG",
        		"ServiceInfo" : {
        	  		"cluster_name" : "c1",
        	  		"service_name" : "HCATALOG"
        	  	}
        	},
        	{
        		"href" : "http://your.ambari.server/api/v1/clusters/c1/services/PIG",
        		"ServiceInfo" : {
        	  		"cluster_name" : "c1",
        	  		"service_name" : "PIG"
        	  	}	
        	}
        ]
    }    