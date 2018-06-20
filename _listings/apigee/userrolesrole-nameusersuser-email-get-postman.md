{
  "info": {
    "name": "Apigee Edge Get Userroles Role Name Users User Email",
    "_postman_id": "701a8012-66d5-4bf5-adef-79fa4f0579b4",
    "description": "Checks user in a given system role",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "ba52b401-c04a-422a-b44c-f14e5ace8b53",
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
              "id": "2a5ab7c1-3b45-4939-a911-7693f2409ef9"
            }
          ]
        },
        {
          "id": "9d6a39cc-eed0-440e-966d-2b1636bd426a",
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
              "id": "c93a7421-c604-458b-9a7e-c3c5e18e2ed5"
            }
          ]
        },
        {
          "id": "f686c2f5-fcb5-4ac9-856d-6c2858e6aa64",
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
              "id": "0c038b20-a04a-46ad-bea9-66e6be3260fa"
            }
          ]
        },
        {
          "id": "8b29d48f-2439-493a-9484-50af67865df2",
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
              "id": "9af2747f-ecc8-4c81-abfa-bcca5ef807e9"
            }
          ]
        },
        {
          "id": "684b00cb-b8bb-4135-869d-d107a3821723",
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
              "id": "fc7058e5-4459-458b-8879-ff57a6bfe95c"
            }
          ]
        },
        {
          "id": "bfd52627-5232-4a94-97f3-3f7b0c877028",
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
              "id": "1bed3759-3cce-4d64-b981-cbb52fa9735b"
            }
          ]
        },
        {
          "id": "f205915f-317c-47e5-9e4d-ae2bc9763adc",
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
              "id": "08092a37-005c-4b78-a754-bffae2a57c8a"
            }
          ]
        },
        {
          "id": "b62594ff-8b49-4150-bed6-a3c74e413457",
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
              "id": "a3d7206b-fb5a-4f94-bb77-37559c6dce7f"
            }
          ]
        },
        {
          "id": "446dfff0-1336-487c-bf9d-b5d07310276a",
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
              "id": "5538b24d-d002-4290-beb7-70710be71858"
            }
          ]
        },
        {
          "id": "e33c12ed-74e4-4079-bf4f-4098d8c89e47",
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
              "id": "2ca2d36d-2d49-4070-a9b9-6a94f086913c"
            }
          ]
        },
        {
          "id": "fac5ebe8-7cd6-459f-b1dc-3a2a9af591bd",
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
              "id": "0fe085bf-b7e6-4b61-9c97-49b37a1fdb65"
            }
          ]
        },
        {
          "id": "339885f7-58a0-4dea-bfbf-7a16c1f408b9",
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
              "id": "1a77a02a-740e-4d05-9feb-7b2f211ff4c6"
            }
          ]
        },
        {
          "id": "2e05d4b5-b268-4715-b461-7592c026e1d0",
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
              "id": "0efe38ef-230b-4376-87e7-abb5f803fcd2"
            }
          ]
        },
        {
          "id": "4c903884-dfda-467f-bf24-79dae350e267",
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
              "id": "72edbd91-d456-4358-85e6-2e4bd855bc01"
            }
          ]
        },
        {
          "id": "3d6280cf-8614-4393-80d4-041bec0e3859",
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
              "id": "6992daee-8d48-493d-a704-7c0df5365856"
            }
          ]
        },
        {
          "id": "9d1f75c1-0c86-4f26-b15b-c50b551da7de",
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
              "id": "7a58e78d-2f5b-4f26-aa29-1be15c28370d"
            }
          ]
        },
        {
          "id": "7fc2a4bb-13bb-4f09-a621-848f107219ec",
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
              "id": "a08e3ae7-13a0-422c-9ea6-23dffd9c183e"
            }
          ]
        },
        {
          "id": "4a3db2ea-80ff-4c47-a399-fecb41842093",
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
              "id": "ef87c424-796f-44de-854a-93a19f305c40"
            }
          ]
        },
        {
          "id": "9ce24e2e-8f16-41cd-97bb-feb65db8b2a1",
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
              "id": "f5c2ae83-0d0e-44b5-8ef8-00336779ace3"
            }
          ]
        },
        {
          "id": "f716c068-34cd-419a-8829-ce138af4a32f",
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
              "id": "767ad9ca-6301-4f47-9a39-0f567608f8cf"
            }
          ]
        },
        {
          "id": "28ff4d0c-d473-4999-8120-3da321631ee8",
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
              "id": "eb037e3e-2ee9-442c-a004-0aa2f4fb838a"
            }
          ]
        },
        {
          "id": "b78dd8be-1a53-42a9-958f-0444ff8d1dc0",
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
              "id": "9add7d46-71aa-438e-b6e8-f46665b3c467"
            }
          ]
        },
        {
          "id": "4f7aeb22-1d4d-4e69-aee0-161b42858221",
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
              "id": "cfa2072c-b917-4cfe-9ae6-788a0e1821ef"
            }
          ]
        },
        {
          "id": "122fe27d-9ab3-46c4-a641-b4b45e16b77e",
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
              "id": "47079d82-53e6-4c5a-b8cb-cff55b4aa34d"
            }
          ]
        },
        {
          "id": "c8bdeedf-cccf-4481-8933-6370c0e7b28e",
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
              "id": "0e05a837-148a-4707-8d06-d2f17358b367"
            }
          ]
        },
        {
          "id": "32f4100b-2672-479b-8b4f-1bf22925db87",
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
              "id": "d0a75628-3e43-4fb6-af9f-43f5326f5d4c"
            }
          ]
        },
        {
          "id": "1f162f12-e491-4b68-8d46-3d571b613aa3",
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
              "id": "8e9b25eb-c9ed-48aa-8a29-7545b14f6a5a"
            }
          ]
        },
        {
          "id": "7a473a89-c057-4fa1-b558-495cf919b6a6",
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
              "id": "6c8a6e1b-e82d-4420-b208-3f524f9e1482"
            }
          ]
        },
        {
          "id": "ef04d828-e139-4014-894e-ccffaba72721",
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
              "id": "c6a0e355-1286-40f1-bf8f-61f542b02828"
            }
          ]
        },
        {
          "id": "1e497eec-4672-4ad1-b38d-eb8697982384",
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
              "id": "9d7be781-b306-4f54-b84f-35d5bd842d43"
            }
          ]
        },
        {
          "id": "7e6b16ca-0ef3-42ed-a069-044b517a6014",
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
              "id": "6695d6d5-f941-4a88-b037-5f2d2e49082a"
            }
          ]
        },
        {
          "id": "a8ac9425-ab0c-427e-a065-cffee24748fd",
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
              "id": "77a52e8c-8684-4313-b45b-289ce93d0d2e"
            }
          ]
        },
        {
          "id": "6974efc8-af1c-49b3-b3eb-d40b125ab022",
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
              "id": "ece79322-6842-4b23-87a2-a8fffd9af4eb"
            }
          ]
        },
        {
          "id": "981def36-c5f3-422e-8461-b0a7cfadee22",
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
              "id": "9b1966e7-2cbc-4a0e-b720-4e3d7e283965"
            }
          ]
        },
        {
          "id": "3759eeff-187b-422a-8560-828c696fd5bf",
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
              "id": "aeca6d17-5c6c-492e-811e-56548049102b"
            }
          ]
        },
        {
          "id": "a61d34c9-342c-4e72-ad58-5e88dcb2bc85",
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
              "id": "30467176-f892-419e-93c8-090541970f22"
            }
          ]
        },
        {
          "id": "6b6d513d-4fd7-4cf5-a8a9-ddcb50b88b93",
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
              "id": "8967f3b9-03ca-4a91-bbc6-26f7d5c296f7"
            }
          ]
        },
        {
          "id": "28d6568e-4354-420b-a0da-cf6b62417d41",
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
              "id": "0174bbc5-48bd-4c20-811e-5232910266f6"
            }
          ]
        },
        {
          "id": "7561dc8a-e49a-43f3-98f1-4707dec0ba1f",
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
              "id": "4f273175-8f65-4d4d-a787-b1391d5ada13"
            }
          ]
        },
        {
          "id": "cdaab963-b3c0-4e79-b0e0-2e85a83110d7",
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
              "id": "b82bd475-6869-4e81-ba63-4246a09df6c6"
            }
          ]
        },
        {
          "id": "f6c5358d-33df-488f-9b2a-538b71b801d3",
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
              "id": "439145b9-d462-4a5b-af20-c1cea2fc6691"
            }
          ]
        },
        {
          "id": "b2e4242f-1de5-447a-92b5-c4ec911a2d0e",
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
              "id": "78cfbb3a-d128-464b-9117-ea97e6ad9bbb"
            }
          ]
        },
        {
          "id": "8a80d99c-4e63-4b9b-b0d7-69ce120853f6",
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
              "id": "f18a7369-b73a-4839-89f5-f76a0734031c"
            }
          ]
        },
        {
          "id": "bee8a42e-5a61-4ac4-94a4-1b1255ad7111",
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
              "id": "25fe419e-1e32-477d-9d69-a8184a50a551"
            }
          ]
        },
        {
          "id": "4fb4c459-a661-4cd0-ac4d-730a8255a038",
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
              "id": "370fcd40-fc10-4cd2-b4b2-2f90ed952820"
            }
          ]
        },
        {
          "id": "8263b514-c0d0-4a65-9425-9a4701fc6137",
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
              "id": "48ee439f-0c12-4baa-a8c9-100ab3b29a55"
            }
          ]
        },
        {
          "id": "647bf65a-b7bf-4475-8d52-051ca6652493",
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
              "id": "1218d7eb-9ad1-4166-b42a-202aa8c46601"
            }
          ]
        },
        {
          "id": "eb643da1-2a0b-4f00-909b-90234d7a0568",
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
              "id": "7432d7c6-6702-4d83-8f2c-9a4612b1f148"
            }
          ]
        },
        {
          "id": "c187c928-538a-4ffe-9afa-6b5e5304d280",
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
              "id": "5041dce2-474e-4469-9e87-a668f1eeba54"
            }
          ]
        },
        {
          "id": "bb01c878-c30f-4e10-b2dc-770d6e952313",
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
              "id": "2be85e85-020e-4498-aa2e-e79cb9bd79b6"
            }
          ]
        },
        {
          "id": "ae25d81d-130a-4297-8add-f08d7f4ce570",
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
              "id": "273c6453-93ff-4831-9e46-7222b676330e"
            }
          ]
        },
        {
          "id": "03b86038-6deb-4342-a061-7ede2fbcbbe1",
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
              "id": "f1fb9bf4-4f2b-48ee-87e7-f3f062bced7a"
            }
          ]
        },
        {
          "id": "cf457a22-9f91-456c-a0af-f48403065979",
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
              "id": "5c02e98f-4da0-476d-88db-1141d930851e"
            }
          ]
        },
        {
          "id": "605eb03e-6da0-42d4-a1dc-beb9ba5fd682",
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
              "id": "96bc50fb-2429-4a02-90ce-c4008c77b97d"
            }
          ]
        },
        {
          "id": "e2601741-b8ce-4df7-b411-4d3d8fd03a7b",
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
              "id": "aa037c38-d5c6-4146-bb32-b38dd22e467e"
            }
          ]
        },
        {
          "id": "dc09d002-a79c-4d06-9702-c6d218886aec",
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
              "id": "67fa0541-a0b6-4539-80b6-a1fa9d7659c0"
            }
          ]
        },
        {
          "id": "357e33fd-11bf-4834-885b-9d0ad3f37288",
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
              "id": "968814da-6e24-4ed9-af19-3b532296b380"
            }
          ]
        },
        {
          "id": "bc7f7920-3312-48a9-9518-eb5eb7964a15",
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
              "id": "949e4afe-1143-4b21-8482-5c465e3911ea"
            }
          ]
        },
        {
          "id": "ce785aa9-3cab-4929-9809-f5208cbe2a03",
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
              "id": "189205c3-ddcb-4c3d-b358-ffaaadd21d76"
            }
          ]
        },
        {
          "id": "aca9f125-ef57-4057-91c4-7d4e60bc9227",
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
              "id": "67d58755-6299-44e3-9854-ce01917ef9c7"
            }
          ]
        },
        {
          "id": "b8f858cd-6b38-437b-bf12-d06210047bad",
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
              "id": "e6b5560c-f10f-49df-8a6f-4b118334df1b"
            }
          ]
        },
        {
          "id": "442ee2f7-6562-4763-b1fd-e6f321514238",
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
              "id": "82e32812-0fa9-4481-8921-edb620b31c01"
            }
          ]
        },
        {
          "id": "e1679d45-43f0-41c5-809c-505a57b27899",
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
              "id": "85a9b874-411a-431e-9a8f-bab7da7e8228"
            }
          ]
        },
        {
          "id": "f25b1c86-b4d3-403e-966d-8556be973452",
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
              "id": "f9d1d282-f6cc-4549-9bda-68696084f8aa"
            }
          ]
        },
        {
          "id": "d7dc7335-22e8-4d1b-931e-48ee050d958c",
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
              "id": "3f76a39a-b925-441b-8079-e8f6b44eaf8d"
            }
          ]
        },
        {
          "id": "e2173b2a-66ae-4528-8967-607b995abb31",
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
              "id": "a6970176-b348-4b8a-85dd-053725fa14be"
            }
          ]
        },
        {
          "id": "44118ebc-c0a0-4db7-ae94-fca1fe5b0051",
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
              "id": "a45c8a95-fe46-4d57-9025-23f3ffba6068"
            }
          ]
        },
        {
          "id": "be3c0f7a-9047-4a58-b720-7ece47e35949",
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
              "id": "9b054b6c-510c-470c-bd77-b6e2d78064db"
            }
          ]
        },
        {
          "id": "873e4eec-f912-40d8-90d8-45225879ff2c",
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
              "id": "6489360e-a713-4bd5-a603-1de1c2090940"
            }
          ]
        },
        {
          "id": "87297fcf-af29-42bb-a709-eb1aaae1b86e",
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
              "id": "14352016-c88a-4cc9-88c9-2eb8086e28cf"
            }
          ]
        },
        {
          "id": "e1a035be-7ecd-4fc6-a643-d9d895b41b82",
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
              "id": "7256e359-b379-4dfc-858f-42402d8c777a"
            }
          ]
        },
        {
          "id": "68b6839f-1445-4671-97da-0290191cc9e7",
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
              "id": "c40a9de2-0727-4a7e-94a2-31fb8970dbe6"
            }
          ]
        },
        {
          "id": "11751535-ac54-4e63-8c2f-a086a3d7de7e",
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
              "id": "e52b1ea5-2b36-42b9-9c19-56640dc409fa"
            }
          ]
        },
        {
          "id": "15e0aaca-5c96-4566-9a38-00b7b25e8e20",
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
              "id": "f16e8c4f-38b8-4833-9d34-f931e69ec2ca"
            }
          ]
        },
        {
          "id": "b7f7445f-77d1-4ba7-83f9-381620b4d34c",
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
              "id": "68ea8f32-3f37-4bf0-9963-81c1bec20b87"
            }
          ]
        },
        {
          "id": "2c247720-04e5-4adf-86c6-8dd3f70d3a78",
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
              "id": "a009370c-ef2e-4f40-aaee-a6fe64721aa8"
            }
          ]
        },
        {
          "id": "2394a37f-a133-4661-a464-8a6d7be472d2",
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
              "id": "caa48473-191e-47e3-bd73-c360b3f23adc"
            }
          ]
        },
        {
          "id": "d01e038a-ff83-4269-8e11-35a0c1dcf34e",
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
              "id": "48410b5b-a682-4d72-8cae-4d3dc3b7ce20"
            }
          ]
        },
        {
          "id": "821f4e82-16f8-45a7-9e0b-d099361e0aff",
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
              "id": "beda2d1d-fc26-430a-8cd8-6fc67facc2f5"
            }
          ]
        },
        {
          "id": "89566f60-d542-4936-b03d-da8cc122096c",
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
              "id": "33eeb9a3-0a93-41bd-bf44-ed8f521e11aa"
            }
          ]
        },
        {
          "id": "fdfcf4e3-d81d-490e-a616-9877c6eb4823",
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
              "id": "afa7049c-2d9a-4550-b549-3a1aa34385f3"
            }
          ]
        },
        {
          "id": "d879f571-d9c0-44f6-a7ce-00bfa5a43070",
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
              "id": "88547d32-800c-48e7-8a6c-461e8d710321"
            }
          ]
        },
        {
          "id": "5620a3fb-3425-40d1-bb0d-8ddaaa2cd576",
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
              "id": "aec78f16-a883-4c73-92a0-f023d1914414"
            }
          ]
        },
        {
          "id": "46b432d3-4d22-4f45-a9dd-f7c161617252",
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
              "id": "cdaebb7c-328a-4710-b76d-8dcab85c5238"
            }
          ]
        },
        {
          "id": "1dcd4af4-2899-4506-8429-f53bc376ecbf",
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
              "id": "b38ffed6-0797-48a2-90a9-42a911b537f6"
            }
          ]
        },
        {
          "id": "ae5863bd-39ad-47c5-a94b-131d3ec6175d",
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
              "id": "139dcb4f-46af-4ccc-bdcb-607663d6f203"
            }
          ]
        },
        {
          "id": "ec03977c-e49b-4a91-8117-a08071a926e2",
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
              "id": "b2ab7dd0-2f7e-49c1-9a7b-364f9a8eecab"
            }
          ]
        },
        {
          "id": "b378edf0-f09d-4d99-87b8-1af8c29156ee",
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
              "id": "b289b953-acfe-4ded-99ae-5060622ba9ff"
            }
          ]
        },
        {
          "id": "141cde02-3206-46cb-868c-ab3fb008515e",
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
              "id": "0a6a0ad2-7848-4324-8175-d6519858ff20"
            }
          ]
        },
        {
          "id": "49899c7f-1bbc-4fc1-970d-68ad7a992528",
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
              "id": "b7c8324a-20e7-4c70-963d-1586f420397d"
            }
          ]
        },
        {
          "id": "1b2bce85-2a45-4fe5-bcfd-8ab1b90c6e1a",
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
              "id": "d5d8a811-741b-4714-8f24-7c4b6ed1c19f"
            }
          ]
        },
        {
          "id": "26d7b475-5548-439b-a6ae-75ddab93fca3",
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
              "id": "f21e49b8-50f9-4ad8-8911-fd4ff6f708fa"
            }
          ]
        },
        {
          "id": "6e97102e-89d2-4182-accd-04bf06731c88",
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
              "id": "6ebc3ffe-0aea-45f5-8f8e-ae10d86f9975"
            }
          ]
        },
        {
          "id": "2c336ffb-9451-423a-be0c-61fdec0af739",
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
              "id": "06173d51-0cad-4a05-b386-88d783191602"
            }
          ]
        },
        {
          "id": "48df816a-c88c-4d64-b51c-180afe90a604",
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
              "id": "b1f98263-f2e3-4821-ac97-0e7216a5867e"
            }
          ]
        },
        {
          "id": "3a30441d-18fe-4d38-9213-b4f29ec88322",
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
              "id": "aad7bbea-02a8-4d83-a0e1-95436b67227f"
            }
          ]
        },
        {
          "id": "237fad5a-253c-427b-9eed-13b76ea55129",
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
              "id": "0e880390-2692-4459-982f-5a0404922a94"
            }
          ]
        },
        {
          "id": "3b1813e4-1739-4502-a574-8fc78f0c684b",
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
              "id": "b176c0d1-9ae1-4dde-94b3-04d52ea87ae9"
            }
          ]
        },
        {
          "id": "3be91022-6068-4155-9dfc-6ffd77560124",
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
              "id": "381ef93c-44d9-49d6-a4d6-f6af80a16552"
            }
          ]
        },
        {
          "id": "43f8bd3b-88b8-48a9-960f-a9d071e25f8c",
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
              "id": "26288f7a-0a67-45e0-884b-cdce2cec2660"
            }
          ]
        },
        {
          "id": "af915a85-6ff5-4b0c-91f2-fb80cab3128d",
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
              "id": "d179a8f7-e76f-401a-9628-7dbf8b52364b"
            }
          ]
        },
        {
          "id": "e8240b0b-c193-45d3-958f-da099dc26052",
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
              "id": "7b85326e-c5c3-416f-9a88-c6ef71ff1593"
            }
          ]
        },
        {
          "id": "7ade239f-340e-426c-b7b5-80513ea044ad",
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
              "id": "aa82e522-2f70-410b-bf63-7d4002cc6171"
            }
          ]
        },
        {
          "id": "3006456b-d825-47d9-9d25-55890c8cc3d8",
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
              "id": "1c0171be-75c6-420f-8121-6847f62d5bb4"
            }
          ]
        },
        {
          "id": "bdf284b2-f2b8-4fa4-ae21-250ce4a77f6f",
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
              "id": "bd97fb01-b2ea-4dba-8a10-0168a4dcac94"
            }
          ]
        },
        {
          "id": "3f707726-2103-4971-94dd-69dcbf948333",
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
              "id": "a806a9ce-22ab-42b2-a0bf-ba008aa08ad7"
            }
          ]
        },
        {
          "id": "6c45bdba-57a6-42d0-b51e-7a002da72c3f",
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
              "id": "80c69ef5-c774-4321-9a3d-b804b34b553b"
            }
          ]
        },
        {
          "id": "d99eab31-dc7c-424f-aa0b-ed058e53baff",
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
              "id": "39549164-39ce-495f-82e5-a9ff6ef31051"
            }
          ]
        },
        {
          "id": "1918124e-47a1-4ee1-a89d-8e07bb5f6178",
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
              "id": "ec994866-0dc6-4857-9b5c-c01bdfb7547d"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizationss",
      "item": [
        {
          "id": "9998a24a-1f03-4d8e-97e6-8678c6df709c",
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
              "id": "687ba9cf-93d9-44e4-a2d3-8eeb7dc87cd2"
            }
          ]
        },
        {
          "id": "aaa84334-6b7d-4718-8117-bb2ff2acafe9",
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
              "id": "c502a716-21f9-4490-8b09-a7c99845c56d"
            }
          ]
        },
        {
          "id": "16abaef5-58dc-413a-975c-9c57e684f2a3",
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
              "id": "87056897-fc32-4e49-8929-e6a4827ba96a"
            }
          ]
        },
        {
          "id": "6f7cb6c4-31e1-453f-b4dc-005acea5d1f7",
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
              "id": "8fd14a33-3a5d-40df-9b29-d088549f47a2"
            }
          ]
        },
        {
          "id": "879effba-7b48-40fc-aa19-b769de04c53e",
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
              "id": "6c48f16f-9b20-4933-9838-52af66348099"
            }
          ]
        },
        {
          "id": "38592d07-33cb-40ee-9ad3-fd4fb028edc0",
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
              "id": "0193c887-af50-4c02-a747-8cf6422a403d"
            }
          ]
        },
        {
          "id": "82dd4289-4b5b-4150-8aa1-88d6dc5ca624",
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
              "id": "bc51429f-504b-4de5-9e00-9e0bcc02edc5"
            }
          ]
        },
        {
          "id": "f69e52ca-3458-4b7d-a397-f603044a3375",
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
              "id": "940f07bc-7062-447f-a9f2-2bcd43edc84b"
            }
          ]
        }
      ]
    },
    {
      "name": "Auditsanizations",
      "item": [
        {
          "id": "2a2e2a1a-e932-4a1a-8c31-dd84a512ab42",
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
              "id": "7139b179-352c-4519-9efe-6d539922c543"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "fa3f8466-4766-43c0-9265-3d867386234c",
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
              "id": "6ad04bfa-3cfa-4ff6-b2d9-ae43a11e3610"
            }
          ]
        },
        {
          "id": "f0f94e7f-f458-47af-b77c-8dc90eb924f2",
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
              "id": "7408e953-cdb5-434d-8eaf-7e85d74bb2be"
            }
          ]
        },
        {
          "id": "19f1f961-d4bb-4576-8a61-0ef26856e3a7",
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
              "id": "de9340e1-3c2a-4453-b81b-862431de77ec"
            }
          ]
        },
        {
          "id": "2ed8809f-9dbd-4523-8dfd-241a40ba0a84",
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
              "id": "fe578e55-52ec-4024-95d2-21d1b8188b66"
            }
          ]
        },
        {
          "id": "71c8ac37-0317-4a5d-88e1-5731f7fe4db3",
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
              "id": "6a89d066-9618-4984-a424-609eb70b4879"
            }
          ]
        },
        {
          "id": "86f6ad12-09c2-4921-a6ed-169a1464d4ec",
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
              "id": "77a01155-4c26-4deb-8e9f-09c48409b205"
            }
          ]
        },
        {
          "id": "7ecea493-318f-4217-b3b0-b0e1be1c79bb",
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
              "id": "8d0cdd96-dd35-4631-9a16-b3ecf5a9cd81"
            }
          ]
        }
      ]
    },
    {
      "name": "Userroles",
      "item": [
        {
          "id": "97afc233-65fa-47ab-af21-e5ee81b90cc2",
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
              "id": "4061157d-b709-49af-bc26-456803ea2b2a"
            }
          ]
        },
        {
          "id": "2635976a-be80-435e-a9ac-fae97cd95823",
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
              "id": "f18b1108-4ba3-4742-af0c-61163e2c22f7"
            }
          ]
        },
        {
          "id": "cf3bf16d-85f4-4612-8afa-1fc23ed770ac",
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
              "id": "30792723-39f7-449d-9712-d454b307e1d7"
            }
          ]
        },
        {
          "id": "507df12b-c150-447d-a962-1d78bb1f3d0e",
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
              "id": "515d8736-fce1-4574-8dd3-37bff6331093"
            }
          ]
        },
        {
          "id": "d6391b30-727e-45b6-b541-43ef42bc765e",
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
              "id": "7a68ec2e-046e-4636-8bf7-e3715097d7e8"
            }
          ]
        },
        {
          "id": "1141dedc-8de0-4092-bb3e-3acd71cc11ab",
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
              "id": "5c214ad1-2704-4e01-8529-1cd408c62c7a"
            }
          ]
        },
        {
          "id": "a79f6f87-b135-45e2-9216-95bdc244cb8f",
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
              "id": "292df78a-1d26-4e31-8a72-b2b288fac81e"
            }
          ]
        }
      ]
    }
  ]
}