{
  "info": {
    "name": "Apigee Edge Get Userroles Role Name Permissions Get",
    "_postman_id": "13cf3e4b-bbf3-473e-97cd-1b2613d4b97e",
    "description": "Checks particular userrole permission for a resource at global level.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "f57e2fa0-c531-4f62-9c19-2e50717e39f1",
          "name": "getOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the organizations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5ba59e7-ea27-40e8-a690-d4fcad2b137c"
            }
          ]
        },
        {
          "id": "bd6af8c1-5c25-4c25-9c9c-f5fc6bd1d392",
          "name": "postOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91988412-c4ee-48e2-afea-fdce89aae512"
            }
          ]
        },
        {
          "id": "de27e631-e1fb-434f-ad3a-4e12bd100a29",
          "name": "getOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3e3f5fb-1df0-43d0-b658-1d4caf74341b"
            }
          ]
        },
        {
          "id": "170bdb59-c8db-431a-a487-d6249bdbbbf2",
          "name": "putOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the description of a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d4703ad-5d5e-48b0-abbe-c62c92bd370d"
            }
          ]
        },
        {
          "id": "33e03711-2b85-4d0d-a624-3eda27de076d",
          "name": "deleteOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11467c4d-7b90-4062-b33c-13e3959e1d98"
            }
          ]
        },
        {
          "id": "7704ad22-186c-4535-a99e-41545b1cd06a",
          "name": "getOrganizationsOrgNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/deployments"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all deployments of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f110f8d2-b684-4a0a-9da2-d750177379fa"
            }
          ]
        },
        {
          "id": "19cabc07-9234-4cfc-bf4e-64d0d7e04c76",
          "name": "getOrganizationsOrgNamePods",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/pods"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pods associated with an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "535c97a6-a393-48cd-a61c-9b408d8afbce"
            }
          ]
        },
        {
          "id": "727925c1-06f7-42e8-ac73-84044891d18d",
          "name": "postOrganizationsOrgNamePods",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/pods"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a pod from an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d302d40a-f134-4382-a651-5dc4fa817c2e"
            }
          ]
        },
        {
          "id": "202da393-d27a-4137-8ef0-f0f33889d541",
          "name": "getOrganizationsOrgNameEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the environments in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2169e84-b54f-4eae-9d14-4514ff4add01"
            }
          ]
        },
        {
          "id": "4c982c91-7cdc-4375-86b7-34b30409aaba",
          "name": "postOrganizationsOrgNameEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f951733-276e-4942-a8e1-3b06574ffc9c"
            }
          ]
        },
        {
          "id": "c9e1ed1e-e72f-4585-918b-f81364ff3a7a",
          "name": "getOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details for an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb9459a6-4ebf-41d3-aff7-5d856d67f2ff"
            }
          ]
        },
        {
          "id": "924a21de-83c7-4b96-a82a-7153ba197120",
          "name": "postOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aec5091e-547a-4ff4-8c8f-8d114fed5a4e"
            }
          ]
        },
        {
          "id": "3485f1b7-1fda-4ddf-a819-da60319624e1",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74de1148-6b3d-4519-b4da-c274183e1701"
            }
          ]
        },
        {
          "id": "2f4d09de-7e09-45ba-bfd4-79a4da9f85fc",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/deployments"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cbb3898-00f2-4736-8d1b-b0a8ae18170a"
            }
          ]
        },
        {
          "id": "f2b79a2d-ef28-4ac1-ae06-49e09c53c50b",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/apis/:api_name/deployments"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an API Proxy in the given environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2c5610f-12af-4d2b-a7a8-4e8ef42a6419"
            }
          ]
        },
        {
          "id": "21815081-a107-4b98-afd1-a8c95a51c8b6",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameRevisionsRevisionNumberDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/apis/:api_name/revisions/:revision_number/deployments"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the deployments for an API Proxyâs revision for an environment in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "021351d7-f282-4e1b-866b-9497afc170ce"
            }
          ]
        },
        {
          "id": "4b50b65c-9b1d-4d04-ae07-e36bc6cb7f68",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the servers that are bound to an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "510d7eac-c553-4007-9f83-28ce94144fb2"
            }
          ]
        },
        {
          "id": "b0df4550-2190-4497-b2bf-a496eae6199a",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add servers into the environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48e480c8-eb63-4f71-832e-4a32c32a9afd"
            }
          ]
        },
        {
          "id": "44887344-206b-47e9-830c-0fff8d785aa2",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvNameServers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/servers"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes servers from the environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3148cc86-61cd-4259-ab35-cadfae08f983"
            }
          ]
        },
        {
          "id": "4a0a69d3-44e8-4ef6-ba5d-1fa4d8b5df53",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all virtual hosts in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a257999-d9ed-4ab4-b0e6-9f4a865f6c5a"
            }
          ]
        },
        {
          "id": "c1a8f88a-8ed3-4158-9aff-70db7cdda87c",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a virtual host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01e826ce-2125-4559-940a-df17934f9a77"
            }
          ]
        },
        {
          "id": "4b9f7365-f894-4bdb-9acf-b28bc4f7aa0e",
          "name": "getOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details for a named virtual host ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fab35106-7e06-48f9-9457-0d432e3fbbf3"
            }
          ]
        },
        {
          "id": "8b7f6790-eb11-4cf7-b8c9-2c33b3fe0000",
          "name": "postOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a specific virtual host in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54649689-4baa-4c9d-9daa-6dcac224adf0"
            }
          ]
        },
        {
          "id": "af8c6fcb-0efa-4870-bfe1-3822f021518b",
          "name": "deleteOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments/:env_name/virtualhosts/:virtualhost_name"
              ],
              "variable": [
                {
                  "id": "env_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualhost_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific virtual host in an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6610ed-c9d7-4d61-8a4d-5fbd39bd26cc"
            }
          ]
        },
        {
          "id": "6813cd52-299f-4916-aa3d-dbc66654358f",
          "name": "getOrganizationsOrgNameApis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all APIs in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "736129d3-bd61-4611-a78d-8a345ce98baf"
            }
          ]
        },
        {
          "id": "4d748cec-52d0-46aa-aa0e-949265b9881b",
          "name": "postOrganizationsOrgNameApis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads a ZIP-formatted API proxy configuration bundle from a local machine to an organization on the API Platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36a24345-727a-470a-9166-0fa19b2b9bf4"
            }
          ]
        },
        {
          "id": "6e963235-9d49-4a86-9daf-3c497342e14f",
          "name": "getOrganizationsOrgNameApiproducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all API products by name for an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa0bb73a-a83b-470b-bc9f-53647c285ad2"
            }
          ]
        },
        {
          "id": "745cfbbb-f4ed-409d-9f93-e0509fc3ad6f",
          "name": "postOrganizationsOrgNameApiproducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an API product: a list of API resources combined with Quota settings that you can use to deliver customized API bundles to your developers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cb5dfa6-3056-46d2-8a90-fef4c58a3e2c"
            }
          ]
        },
        {
          "id": "c1e300e3-b02d-469e-9dee-bb98ed720fa6",
          "name": "getOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the list of keys/apps/developers for an API product of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49c434a8-2463-4643-bb7f-c23497bd1682"
            }
          ]
        },
        {
          "id": "abec6dbb-f4dd-4a4f-b638-375e335b0498",
          "name": "putOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This method updates an existing API product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b77ee208-3661-405b-b1c9-ac5060726179"
            }
          ]
        },
        {
          "id": "3a9d3775-62b8-47c7-bd8c-9970a2dfae0c",
          "name": "deleteOrganizationsOrgNameApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apiproducts/:apiproduct_name"
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an API product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2d41b19-5106-4d84-96a4-2304fd93ba53"
            }
          ]
        },
        {
          "id": "bdd1a8d9-ee5b-4f13-9954-9a49659999d3",
          "name": "getOrganizationsOrgNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers"
              ],
              "query": [
                {
                  "key": "registeredat",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the developer profile by registered date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9deb15d4-52df-4a96-8dae-2b0e0a6542a7"
            }
          ]
        },
        {
          "id": "09c04558-fda4-45bd-863d-a88c9ef9b8cb",
          "name": "postOrganizationsOrgNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a developer in an organization ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46f98783-dd1d-4165-9dec-d5a7e54c4f0d"
            }
          ]
        },
        {
          "id": "9151462b-214d-446a-be31-bdb083deff17",
          "name": "getOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a count of apps by developer email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3a02df4-06cc-4443-a7df-33e6263573f2"
            }
          ]
        },
        {
          "id": "58af3a1b-717c-48e8-8a06-5377896e837a",
          "name": "putOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing developer profile with new values or additional attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b85a95a-6698-46fb-84be-6a813bf82e33"
            }
          ]
        },
        {
          "id": "840ff9e2-6568-4126-80e3-d674cdb3b58a",
          "name": "postOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the status of a developer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "628cb7c3-9808-4ecc-9094-d1d99cf10fcf"
            }
          ]
        },
        {
          "id": "50466793-a59a-48fc-9fa9-685c3245dd74",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_name"
              ],
              "variable": [
                {
                  "id": "developer_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a developer from an Organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e32a475f-2549-49db-afbe-67deebce8d68"
            }
          ]
        },
        {
          "id": "3799ce80-8e69-4c31-bd82-5e3ed6979937",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides an expanded view of a developer's collection of apps ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a8b6a35-b13c-4442-942f-ecd2967c8b9a"
            }
          ]
        },
        {
          "id": "442119f8-2545-48cd-9c8b-9d5e20244302",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app associated with a developer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4328367b-e5f3-4ea6-868a-6f9cfdb4c3f3"
            }
          ]
        },
        {
          "id": "0769b14b-380c-43a0-b9de-4023573c0bb9",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a count of all API resources in the API products accessible by a developer app ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a42210af-a70c-49d7-887b-e265e04c8e7e"
            }
          ]
        },
        {
          "id": "6528bcd6-d7e8-48cf-b639-664456cda4fc",
          "name": "putOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the app to get a new set of consumer credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b74c16c-3bc2-4c5f-b4d5-d6fb1baaea6a"
            }
          ]
        },
        {
          "id": "4a6dbee8-9f64-40a8-a821-3b72c95ff669",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes a Developer App, disabling access to all API Products ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9eb8b32d-828a-4212-8ad1-f2b151fe7bd1"
            }
          ]
        },
        {
          "id": "e74af737-a045-4f85-8faf-a92b7a027c41",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a Developer's App."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c61339b-93b3-4c5a-ae3d-cddeed153969"
            }
          ]
        },
        {
          "id": "dcffb33b-eaa5-4dc4-ae2c-23095f79e9e4",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details for a consumer key for a developer app ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dad6dbf3-9f26-4222-8b90-ad170928b246"
            }
          ]
        },
        {
          "id": "8eca556d-40d4-4f1c-94df-8989736f9428",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes a developer app key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "284866aa-0c72-4f79-9531-a54be333d847"
            }
          ]
        },
        {
          "id": "0ff42cb3-a265-4c80-90c6-1af90862915c",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a consumer key that belongs to an app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ac1df96-7c44-40a2-a548-4d2d22c9c573"
            }
          ]
        },
        {
          "id": "df3f67cc-2a49-4a62-a7f4-ed224a5309bc",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/apiproducts/:apiproduct_name"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes the association of an API Product with a Developer App's consumer key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd20939-7cf0-468b-9eeb-acc3e44a404b"
            }
          ]
        },
        {
          "id": "e5463a5f-5a0e-48f1-afc7-9078a447cf33",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductNam",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/apiproducts/:apiproduct_name"
              ],
              "variable": [
                {
                  "id": "apiproduct_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an API product from a developer app key profile, and thereby renders the developer app unable to access the URIs defined in the API product specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3edbbd3b-16e7-4b59-a241-cba18911ca95"
            }
          ]
        },
        {
          "id": "75581289-9bf8-4716-ab00-acc18ea4357e",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth1accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/oauth1accesstokens"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of OAuth 1.0 access tokens for a developer's app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f58ad1bd-48ae-4b23-a775-b5a9854cbc28"
            }
          ]
        },
        {
          "id": "1c3b3dd8-4b62-4ebd-8c46-82958bddc081",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth2accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/oauth2accesstokens"
              ],
              "query": [
                {
                  "key": "appName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "developerEmail",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "organizationName",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "org_name",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "developer_email",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "app_name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of    OAuth 2.0 access tokens for a developer's app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1878e1b6-cccc-43b7-a843-84bf833d91d0"
            }
          ]
        },
        {
          "id": "41dabfc9-f32d-413b-9fd2-30e5b6a8fa9b",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth1accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/oauth1accesstokens"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of OAuth 1.0 access tokens for a developer's app key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9024783-46d9-4fa9-9ca6-6ed2e93452ce"
            }
          ]
        },
        {
          "id": "45689a48-1fa1-4f13-b3c3-7c2803e2bcef",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth2accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/apps/:app_name/keys/:consumer_key/oauth2accesstokens"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of OAuth 2.0 access tokens for a developer's app key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a57163c0-5748-415a-81bc-24a134cfc804"
            }
          ]
        },
        {
          "id": "cbf7ae3f-4530-40bb-970f-c10f6dd36ffd",
          "name": "getOrganizationsOrgNameOauth1RequesttokensRequestToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/requesttokens/:request_token"
              ],
              "query": [
                {
                  "key": "consumerKey",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "request_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the Oauth 1.0 a request token for the speficied consumer key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a7e07e4-2c20-45d0-a1ad-c780fe51e4c1"
            }
          ]
        },
        {
          "id": "7f7ff573-a116-463e-afb3-191836fb1ee1",
          "name": "postOrganizationsOrgNameOauth1RequesttokensRequestToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/requesttokens/:request_token"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "request_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes an OAuth 1.0 a request token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35dc0b53-d54e-4f4d-9b60-e67dee82e4b8"
            }
          ]
        },
        {
          "id": "7c88d9f1-054a-4e93-a84a-ba972d0ecc3b",
          "name": "deleteOrganizationsOrgNameOauth1RequesttokensRequestToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/requesttokens/:request_token"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "request_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the request token specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e311cad-9f9b-4d39-9e7d-5b3a62bf1d30"
            }
          ]
        },
        {
          "id": "0ce17a9e-dca9-436f-bc0c-8b967a670291",
          "name": "getOrganizationsOrgNameOauth1Requesttokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/requesttokens"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of all OAuth 1.0a request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d814c0a-cd22-4896-8b29-2c124844eb95"
            }
          ]
        },
        {
          "id": "989d37ca-9691-43ee-b2a6-b817c0f6487c",
          "name": "getOrganizationsOrgNameOauth1VerifiersVerifierCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/verifiers/:verifier_code"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "verifier_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the detail of given verifier code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f5adcbf-81e2-4c73-aa6b-5bd3a461e8a3"
            }
          ]
        },
        {
          "id": "ded44cb0-6ca3-4ab2-9033-1be95ba7d71e",
          "name": "deleteOrganizationsOrgNameOauth1VerifiersVerifierCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/verifiers/:verifier_code"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "verifier_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified verifier code, which is the verifier code given by the provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef4028b2-25fd-473b-a17f-5adb18933fbc"
            }
          ]
        },
        {
          "id": "4ea636b5-2b07-4c6b-b2f0-dedd99c364b2",
          "name": "getOrganizationsOrgNameOauth1Verifiers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/verifiers"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all verifiers and details for each verifier in an Organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83f1fcaa-0b01-4250-9284-fea724358435"
            }
          ]
        },
        {
          "id": "16a66ae4-000b-4e39-87b6-5ebbaccb33b6",
          "name": "getOrganizationsOrgNameOauth1AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/accesstokens/:access_token"
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the details of given access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84f02052-4eef-4f9a-89d3-7ebc90d22601"
            }
          ]
        },
        {
          "id": "ebdc069b-6462-4287-95bc-0b4ba295c030",
          "name": "postOrganizationsOrgNameOauth1AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/accesstokens/:access_token"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes the specified access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b8f7ca7-edf9-444e-bedd-e3fc4d3a7f4f"
            }
          ]
        },
        {
          "id": "9b4b2d78-aa52-4c28-8f21-e97864779a0c",
          "name": "deleteOrganizationsOrgNameOauth1AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/accesstokens/:access_token"
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d417495a-7f48-4853-bb1d-7eb72121b7cd"
            }
          ]
        },
        {
          "id": "119b458f-8e4d-4ad6-9448-3956f4bcb5a7",
          "name": "getOrganizationsOrgNameOauth1Accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth1/accesstokens"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a count of all 1.0a access tokens in an orgnization ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01ed5fbd-ef7d-452a-b7d8-b08cd2c7609e"
            }
          ]
        },
        {
          "id": "6dc3ccde-5eb4-4415-89ce-469da0044fae",
          "name": "getOrganizationsOrgNameOauth2AuthorizationcodesAuthorizationCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/authorizationcodes/:authorization_code"
              ],
              "variable": [
                {
                  "id": "authorization_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a specific Authorization Code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87ede32d-595f-4c47-aa50-8fceda263ba4"
            }
          ]
        },
        {
          "id": "e1091d19-14e6-4338-ae17-ce9cdc27e3f1",
          "name": "deleteOrganizationsOrgNameOauth2AuthorizationcodesAuthorizationCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/authorizationcodes/:authorization_code"
              ],
              "variable": [
                {
                  "id": "authorization_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the given authorization Code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43eea76d-971b-492e-bd7d-13a604262c35"
            }
          ]
        },
        {
          "id": "ed28bfa6-5b3e-47d6-8f76-9b7b1a52d308",
          "name": "getOrganizationsOrgNameOauth2Authorizationcodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/authorizationcodes"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all authorization codes in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1692f41-2202-4b5a-ac61-49c39f278345"
            }
          ]
        },
        {
          "id": "988d1044-4bea-4441-a458-2ac621c9ba32",
          "name": "getOrganizationsOrgNameOauth2AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/accesstokens/:access_token"
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details of a specific access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f70a5a6d-c41a-40c3-a83f-b27829dacd40"
            }
          ]
        },
        {
          "id": "a4161ee1-b31c-45a9-b897-4bb9265053ec",
          "name": "postOrganizationsOrgNameOauth2AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/accesstokens/:access_token"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes a specific access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c199578-3c52-4852-aa27-79dedff3a892"
            }
          ]
        },
        {
          "id": "c99baaed-6236-4dd4-9742-cc66680748b8",
          "name": "deleteOrganizationsOrgNameOauth2AccesstokensAccessToken",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/accesstokens/:access_token"
              ],
              "variable": [
                {
                  "id": "access_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific access token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "560ad653-9aa1-4045-9211-4f298d9a99b5"
            }
          ]
        },
        {
          "id": "b23d4620-3d25-470e-a2f7-8bbc4eaeadfe",
          "name": "getOrganizationsOrgNameOauth2Accesstokens",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/oauth2/accesstokens"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get count of OAuth 2.0 access tokens under an organization ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92084aa4-21fe-492c-825d-33776f4914a4"
            }
          ]
        },
        {
          "id": "a98ea46d-5b3d-4764-a144-826723368097",
          "name": "getOrganizationsOrgNameKeyvaluemaps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an expanded view of all Maps scoped by organization, environment or API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "320ce753-8194-4735-bb9f-1b91cc907499"
            }
          ]
        },
        {
          "id": "d169aab3-974c-4850-9412-fbe255a2449e",
          "name": "postOrganizationsOrgNameKeyvaluemaps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a KeyValueMap."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "530f5797-4f76-4596-9525-c3f958198010"
            }
          ]
        },
        {
          "id": "c4bc1e4c-a892-4d9f-8ab8-627cf4637fb6",
          "name": "getOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps/:map_name/entries/:entry_name"
              ],
              "variable": [
                {
                  "id": "entry_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "map_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific entry details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bf32245-7cf8-4cb8-9448-4746d67d3886"
            }
          ]
        },
        {
          "id": "be4df95f-990a-4a8c-9a27-48fbf75a2223",
          "name": "deleteOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps/:map_name/entries/:entry_name"
              ],
              "variable": [
                {
                  "id": "entry_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "map_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a single entry by name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93774cf0-5a4b-4352-87e6-0ca1a564e22d"
            }
          ]
        },
        {
          "id": "d6e4895e-1fa9-4534-b6a8-afd57c78d034",
          "name": "getOrganizationsOrgNameKeyvaluemapsMapName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps/:map_name"
              ],
              "variable": [
                {
                  "id": "map_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a KeyValueMap by name, along with associated entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e3ee281-0214-4ba0-a751-3ae28727d3bb"
            }
          ]
        },
        {
          "id": "3b41cc5a-94a6-4b03-82e9-093ed348a0cf",
          "name": "putOrganizationsOrgNameKeyvaluemapsMapName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps/:map_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "map_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing KeyValueMap."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e991f47c-8916-4c59-8a52-d599f8396cc0"
            }
          ]
        },
        {
          "id": "3991df43-9f00-439c-b652-0167f6484a82",
          "name": "deleteOrganizationsOrgNameKeyvaluemapsMapName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/keyvaluemaps/:map_name"
              ],
              "variable": [
                {
                  "id": "map_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a KeyValueMap and all associated entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2d90326-0018-4e23-9589-50bd1018bba8"
            }
          ]
        },
        {
          "id": "7deb6686-36f5-4135-a499-349a29d8475a",
          "name": "getOrganizationsOrgNameCompanies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an expanded list of companies, displaying a full profile for each company in the organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb574fe0-536f-4460-841f-9e4ce76ba1e8"
            }
          ]
        },
        {
          "id": "21f64e59-026c-430b-8ab1-03bbc7a320b9",
          "name": "postOrganizationsOrgNameCompanies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a company in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be1db6eb-421c-4295-8528-14cbd3dbc4e2"
            }
          ]
        },
        {
          "id": "8f067f0b-b58b-4eb9-b9eb-1e4717e18c73",
          "name": "getOrganizationsOrgNameCompaniesCompanyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name"
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details for a Company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6276e5c2-a698-4266-a385-7566bb85d038"
            }
          ]
        },
        {
          "id": "99eee8b4-3202-40ed-b512-80ca21640412",
          "name": "putOrganizationsOrgNameCompaniesCompanyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing Company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "131caaa8-4b85-41a1-a58c-6a99fd33e827"
            }
          ]
        },
        {
          "id": "06e28368-d25f-4725-b374-928fc4fd6e42",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name"
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing Company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72d2ab94-16b2-450a-9c36-c2ce18e6c5e1"
            }
          ]
        },
        {
          "id": "ee934f6d-c090-433e-ae74-715b1ab2137c",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/developers"
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all developers associated with a company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3de7780a-526a-4d55-bbfc-e7e36c18e846"
            }
          ]
        },
        {
          "id": "ec6424f6-fc29-4395-ac52-f25a3a42073e",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameDevelopers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/developers"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a developer to a company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2391b58-7814-4cc4-9756-729c26991b12"
            }
          ]
        },
        {
          "id": "40c78e8f-7d41-434a-9577-d7968a7f6ba4",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyNameDevelopersDeveloperEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/developers/{developer_email}"
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "Developer_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the association of a Developer with a Company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6e5364e-9af1-4e1f-8499-0f7d1ac9da8e"
            }
          ]
        },
        {
          "id": "3f198e94-2917-48c7-8ad2-0973c2c3547a",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an expanded list company apps ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9051f0c0-52fb-4f3d-8697-df9a950809c2"
            }
          ]
        },
        {
          "id": "7ef8d716-509a-488e-8921-b4d8334cfc29",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameApps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app for a company."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "482b4a39-92cb-4a26-92a5-cea7320b29c2"
            }
          ]
        },
        {
          "id": "95463ef8-b625-4615-af6a-ccadf91f3f4a",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name"
              ],
              "query": [
                {
                  "key": "entity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "query",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the count    of API resources for a company app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af29fc8a-4c90-4089-8e81-a4fdf258d72d"
            }
          ]
        },
        {
          "id": "94eb5b29-0c32-4a98-ad8e-4a7e83279e7e",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing company app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88468bcf-5f41-4529-b39d-f75e2b2433dd"
            }
          ]
        },
        {
          "id": "c16e589f-e38d-4ca2-98a8-56f1d2ea922d",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyNameAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a company app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "600a5951-83b0-436e-ba2a-44c9faeba1b7"
            }
          ]
        },
        {
          "id": "b51288ce-ef83-41b8-81cf-3635edf761d9",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the consumer key issued to a company app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaff6099-b15a-4955-941d-c787652ba04a"
            }
          ]
        },
        {
          "id": "e6303cdb-9aba-4d02-98be-b4ff1e923ab2",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name/keys/:consumer_key"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Revokes the specific key of a company app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "743a66b7-c784-4c87-8431-6232f0df794d"
            }
          ]
        },
        {
          "id": "dec4dde2-fbb6-43ed-863d-d48b310d9849",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/apps/:app_name/keys/:consumer_key"
              ],
              "variable": [
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "consumer_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a company app key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb2c9b92-e897-4e6a-b507-1af6b36e4421"
            }
          ]
        },
        {
          "id": "13c9f11b-6d13-426d-8ede-71f6ce79c768",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameAppfamilies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies"
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An expanded list of all app families in an organization, listing Apps in the collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41d83917-df6e-4f19-aeae-44212151032f"
            }
          ]
        },
        {
          "id": "9834395a-2b0e-4169-a212-daf07b7de63a",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameAppfamilies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee7ca191-d46a-422f-b4e0-e4e2e2e0c9e8"
            }
          ]
        },
        {
          "id": "aeaa4957-2b3c-4814-9135-d7d37783ef23",
          "name": "getOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies/:appfamily_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of apps in an appfamily."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04cb63b0-559d-428d-86dd-d1fae502b21b"
            }
          ]
        },
        {
          "id": "38157afc-5fe1-4ecf-8389-aaf12b72276e",
          "name": "postOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies/:appfamily_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing app family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44bbe2ff-c4f2-4ef7-8eea-3b4dc292f173"
            }
          ]
        },
        {
          "id": "3c0be960-a8cf-469a-a362-78c75f43590a",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies/:appfamily_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an App Family and all Apps it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97790fe2-3e0d-4740-a93a-7ad86613c1e9"
            }
          ]
        },
        {
          "id": "8e1dc277-c8b7-4200-b33c-8bb66d6e8299",
          "name": "deleteOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyNameAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies/:company_name/appfamilies/:appfamily_name/apps/:app_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "company_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an App from an App Family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d61883e0-547d-4920-8c72-6fed9c844bb7"
            }
          ]
        },
        {
          "id": "7b67ddba-fe46-422c-97a1-d7d8b7318ffb",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppfamilies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies"
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "An expanded list of all app families in an organization, listing Apps in the collection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8368a376-7fc4-4b0c-a7fb-688fe7427286"
            }
          ]
        },
        {
          "id": "797c2251-1f07-4a5d-ae67-76681b271080",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppfamilies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app family for developers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ef74d27-e8dc-40b6-9163-434f9c13f4fd"
            }
          ]
        },
        {
          "id": "70d56fb5-3489-4f6f-b02e-2252b00db446",
          "name": "getOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies/:appfamily_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of apps in an appfamily."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a702f675-292a-441d-9b5c-4e13da8c7d23"
            }
          ]
        },
        {
          "id": "636a3976-0a8b-4dc5-b40b-9b53c7421e98",
          "name": "postOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies/:appfamily_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing app family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d753f6e-feab-4d57-8f7f-faa2cc4978da"
            }
          ]
        },
        {
          "id": "b22929d8-d2e1-4488-9865-ffa3483330f9",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies/:appfamily_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an App Family and all Apps it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedb2af3-91e4-4424-b150-7ee16edc51f8"
            }
          ]
        },
        {
          "id": "8dc4cf4d-9a37-4303-ac52-a220d805f7bf",
          "name": "deleteOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyNameAppsAppName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/developers/:developer_email/appfamilies/:appfamily_name/apps/:app_name"
              ],
              "variable": [
                {
                  "id": "appfamily_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "app_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "developer_email",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an App from an App Family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7566ab9-6552-41f7-bc36-11f3071b672a"
            }
          ]
        },
        {
          "id": "2f267978-d33e-4827-a196-80afab95ed75",
          "name": "getOrganizationsOrgNameUserroles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of roles available to users in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5213dd63-5cef-46b0-bd4b-9aede3ec0fbe"
            }
          ]
        },
        {
          "id": "80b6641f-b587-4742-8243-55581638a3d8",
          "name": "postOrganizationsOrgNameUserroles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a role in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6a09740-5359-4ea1-81df-86ca60ed98b7"
            }
          ]
        },
        {
          "id": "f2ffbf6b-19d7-4042-97d8-43cb36a7e1a0",
          "name": "getOrganizationsOrgNameUserrolesRoleName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "171ab6cb-9773-48f1-a74e-580019e04beb"
            }
          ]
        },
        {
          "id": "c4587bd8-52c9-4674-b8fe-4e27bf477be6",
          "name": "deleteOrganizationsOrgNameUserrolesRoleName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a role from an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "116ed403-2c39-4990-a524-895f94d1ff13"
            }
          ]
        },
        {
          "id": "c33491d4-4303-49fd-aaaa-9bcd1838a78f",
          "name": "getOrganizationsOrgNameResources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/resources"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a RBAC resource based on resource path."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5f11421-8bea-4e4a-8bb9-f6d01c093543"
            }
          ]
        },
        {
          "id": "18322310-67d5-48c8-88bc-18f20c867506",
          "name": "postOrganizationsOrgNameResources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/resources"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd56d0a3-bbd4-454f-abd9-039b647c43a8"
            }
          ]
        },
        {
          "id": "7ec8efe1-84a2-4a87-980a-d688f86b1203",
          "name": "deleteOrganizationsOrgNameResources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/resources"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64d873c5-1761-4326-ba06-041764aefebc"
            }
          ]
        },
        {
          "id": "339e2ef6-f620-4ac7-8741-65579ff7333d",
          "name": "getOrganizationsOrgNameUserrolesRoleNamePermissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name/permissions"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of permissions associated with the specified resource for a single resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41dd5cf1-811d-4b0c-8804-5522eb16e391"
            }
          ]
        },
        {
          "id": "a5a33584-7405-4296-af6e-4264cf964c1e",
          "name": "postOrganizationsOrgNameUserrolesRoleNamePermissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name/permissions"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Associates permissions for a resource with a user role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "260b9738-861c-43c7-961b-71e22f8d0d49"
            }
          ]
        },
        {
          "id": "0fc83e7f-b904-4b91-b92e-f6fbc33d7767",
          "name": "getOrganizationsOrgNameUserrolesRoleNamePermissionsGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name/permissions/get"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the particular userrole permission of a resource at organization level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3e7b77c-dd8d-426f-89f0-76cb6cd5fa5d"
            }
          ]
        },
        {
          "id": "7d331f29-ef15-4e2a-bf7b-e69ba10da3ad",
          "name": "deleteOrganizationsOrgNameUserrolesRoleNamePermissionsGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name/permissions/get"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes particular userrole permission at organization level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "283c8a06-5491-473c-987c-958fa6d0032a"
            }
          ]
        },
        {
          "id": "7ab16909-3c62-4531-b85d-a5f697b1809e",
          "name": "postOrganizationsOrgNameUserrolesRoleNameResourcepermissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/userroles/:role_name/resourcepermissions"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds multiple resource permissions for resource at organization level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f56b3959-ae3b-4887-acbe-efe653b09c5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizationss",
      "item": [
        {
          "id": "14eb79bb-7dd2-4309-be05-8b1b21e9346f",
          "name": "postOrganizationsOrgNameApisApiNameRevisionsRevisionNumberDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/revisions/:revision_number/deployments"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "env",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Undeploys an API proxy revision from an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50a8f776-7752-4263-9bb1-b40613073d79"
            }
          ]
        },
        {
          "id": "338e142c-57fe-45aa-9bcd-333ccadc9dbd",
          "name": "getOrganizationsOrgNameApisApiName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an API proxy by name, providing a list of existing revisions of the API proxy configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ef127cc-c3a2-4f3d-b194-6c3397701e0e"
            }
          ]
        },
        {
          "id": "5926db96-8779-462e-91fc-b39f82ae8170",
          "name": "deleteOrganizationsOrgNameApisApiName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an API and all associated endpoints, policies, resources, and revisions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b630cbc3-6f41-470f-86a4-47d6b0026502"
            }
          ]
        },
        {
          "id": "7154ac59-4b7b-4138-aa77-d70afc355691",
          "name": "putOrganizationsOrgNameApisApiNameRevisionsRevisionNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/revisions/revision_number"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "revision_number",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Use the POST method to update a specific API proxy in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c4b3a57-206b-4d69-871f-f92c88a5653e"
            }
          ]
        },
        {
          "id": "e352025c-4c7a-445e-a974-615ec5678424",
          "name": "getOrganizationsOrgNameApisApiNameRevisionsRevisionNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/revisions/:revision_number"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Exports an API from Apigee to the local machine a ZIP bundle of config and code files.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef8f628a-e5f7-4409-9bd4-c620f7b32d41"
            }
          ]
        },
        {
          "id": "7b0e018b-5c1c-4664-9f93-1e30ac34e3a5",
          "name": "deleteOrganizationsOrgNameApisApiNameRevisionsRevisionNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/revisions/:revision_number"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific revision of an API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80663465-3fcd-499c-bff2-483482efc0ac"
            }
          ]
        },
        {
          "id": "b4a415ef-f2c6-4b0b-9496-483bdea7161f",
          "name": "getOrganizationsOrgNameApisApiNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/deployments"
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detail on deployments of the API specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6924ca4-db0b-4f5b-8a6f-715585c4d123"
            }
          ]
        },
        {
          "id": "92d484df-de65-4881-bdf9-bfd93950fa5a",
          "name": "getOrganizationsOrgNameApisApiNameRevisionsRevisionNameDeployments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/apis/:api_name/revisions/:revision_name/deployments"
              ],
              "query": [
                {
                  "key": "revision_number",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "api_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "revision_name",
                  "value": "revision_name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get deployments for a revision of an API proxy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bead147a-462f-42f4-b190-3fa99e6e49cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Auditsanizations",
      "item": [
        {
          "id": "5408f2b5-bcaa-4106-b76e-1584acf692d3",
          "name": "getAuditsOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "audits/organizations/:org_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists and expands audit records for management operations against APIs, API revisions and policies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8e009e9-7b02-4e6a-a323-ef4741948da2"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "d02d6687-4676-4b80-8b27-42956f7dc098",
          "name": "getUsers",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/users",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7abe2b6-676d-4549-a7e1-0649ca359acd"
            }
          ]
        },
        {
          "id": "8ff6305f-c42d-400e-80e1-10860780d5bb",
          "name": "postUsers",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/users?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d21877de-1f73-4bdc-ac71-828e56441815"
            }
          ]
        },
        {
          "id": "bfe2337b-0874-4a99-8c32-e4d8dab1270c",
          "name": "getUsersUserEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email"
              ],
              "variable": [
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e081b75f-c8c0-4fcd-8035-1381d943ab0e"
            }
          ]
        },
        {
          "id": "e853c6d5-12fb-473b-b226-2816d4e048f8",
          "name": "postUsersUserEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3040544b-37b2-4b25-8523-675793a2246d"
            }
          ]
        },
        {
          "id": "0d51b18e-c168-4e57-8a49-ef62a723a6a7",
          "name": "deleteUsersUserEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email"
              ],
              "variable": [
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd203e46-bc28-4d16-b240-9e629af6dd9f"
            }
          ]
        },
        {
          "id": "e4e109f4-560b-4c57-bbcb-bd95dbea6d25",
          "name": "getUsersUserEmailUserroles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email/userroles"
              ],
              "variable": [
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets roles for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "661be2c4-b42a-450a-b9e4-f68113bbdb32"
            }
          ]
        },
        {
          "id": "8b55fe22-83b2-4bac-9d5c-6d0dfae6bc6d",
          "name": "postUsersUserEmailUserroles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email/userroles"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a user with a organizational user role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e75dbf3-0f7b-4fe5-ac83-45969f40635b"
            }
          ]
        },
        {
          "id": "a545dbbc-28c3-4346-a747-643671453686",
          "name": "deleteUsersUserEmailUserrolesRoleName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "users/:user_email/userroles/:role_name"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "org",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes organizational role for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f818b56c-6b10-46b2-bfb7-5f923fa1657d"
            }
          ]
        }
      ]
    },
    {
      "name": "Userroles",
      "item": [
        {
          "id": "da27c156-7e88-44c6-a69a-f1f0bb0f0047",
          "name": "getUserroles",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/userroles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of roles available to users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0dee59b8-d531-4712-ac24-b7a2fac7f9f8"
            }
          ]
        },
        {
          "id": "861c2eca-67c9-4639-bbba-76b57c75d351",
          "name": "postUserroles",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/userroles?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a role at global level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80ba0c53-80b7-44de-a232-9e66f2cce185"
            }
          ]
        },
        {
          "id": "205984e9-3b1c-4190-bfcf-25c7b8f6be10",
          "name": "getUserrolesRoleName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51118937-aa80-4e42-9698-6ebe0afc6aaa"
            }
          ]
        },
        {
          "id": "b59e214c-9fbb-46cc-9a0d-20c7698f8303",
          "name": "deleteUserrolesRoleName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6174fc66-7655-4715-b48f-1f8aa4e88140"
            }
          ]
        },
        {
          "id": "017ca99f-c38b-4077-8ad1-27c9e6382fd8",
          "name": "getUserrolesRoleNameUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/users"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists users for a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53a8e3e1-c798-4b7f-b4f7-807e2404c540"
            }
          ]
        },
        {
          "id": "9a1fb96a-abdf-463e-978f-7dc7e711a991",
          "name": "postUserrolesRoleNameUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/users"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds user to role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8589191c-0672-47cd-ab30-e9aa40121096"
            }
          ]
        },
        {
          "id": "2a727887-e531-4d38-a8d6-32bf10b43f06",
          "name": "getUserrolesRoleNameUsersUserEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/users/:user_email"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks user in a given system role"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c41eb35d-6e1b-418d-a507-1eabc6952165"
            }
          ]
        },
        {
          "id": "ff1efa6f-5962-43ed-903b-250d1d1f6e8a",
          "name": "deleteUserrolesRoleNameUsersUserEmail",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/users/:user_email"
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_email",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes user for a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68467034-4d10-4e5b-988d-53bb138e73b0"
            }
          ]
        },
        {
          "id": "e255d353-2a3e-4bbb-ae31-cdcabe520bf1",
          "name": "getUserrolesRoleNamePermissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/permissions"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets permission for a specific resource at global level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f3b66da-b485-4aa4-af13-81e94b1ff8e2"
            }
          ]
        },
        {
          "id": "24d10a5d-0e7c-4345-b98c-556e69ca6ed8",
          "name": "postUserrolesRoleNamePermissions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/permissions"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds permissions for resource at global level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b1232d1-f96c-43a9-9733-246cd93ca188"
            }
          ]
        },
        {
          "id": "9bf1f944-c88f-434c-bea6-7b9f4ca869e0",
          "name": "getUserrolesRoleNamePermissionsGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "userroles/:role_name/permissions/get"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "path",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "role_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks particular userrole permission for a resource at global level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "487e042a-3a3b-4b12-99a1-a7171823773b"
            }
          ]
        }
      ]
    },
    {
      "name": "Resources",
      "item": [
        {
          "id": "4fee2733-006d-48be-9a59-68bb4363ba1e",
          "name": "getResources",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/resources?Content-Type=%7B%7D&path=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "339ddfed-4c21-471c-8800-45509461498a"
            }
          ]
        },
        {
          "id": "1cdb2868-baec-4267-a26e-c3bd50a6b52f",
          "name": "postResources",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/resources?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a global level resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee87c329-f209-4fea-93ca-f0866501cf5f"
            }
          ]
        },
        {
          "id": "4603024e-8ef9-4aaf-a5c7-f91efb6ab9d9",
          "name": "deleteResources",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/resources?Content-Type=%7B%7D&path=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99860abe-8d97-480f-8327-9ec929fc1e61"
            }
          ]
        }
      ]
    }
  ]
}