{
  "info": {
    "name": "Apigee Edge Get Users",
    "_postman_id": "d244a33b-7038-41e9-b15e-d0fdf04cdac9",
    "description": "Gets a list of users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "8c08dadf-4e23-4641-a1da-8bab845e0456",
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
              "id": "62f4df89-54c8-4e20-817f-9d49448e51bd"
            }
          ]
        },
        {
          "id": "22238ef5-eea1-4f77-ace7-34bacd3cd40f",
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
              "id": "c9f950b7-3db3-47f6-9be4-43c3c9ff2b15"
            }
          ]
        },
        {
          "id": "ac1abdd3-e591-4c6e-a23f-57f0f89e234b",
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
              "id": "d812964a-5c67-4490-84f4-179a209fa2b3"
            }
          ]
        },
        {
          "id": "45409a99-347d-4d58-8984-a0bd8aa445df",
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
              "id": "a8d6425c-12e2-4c71-b8ee-fcff974f9613"
            }
          ]
        },
        {
          "id": "d2d6acff-1169-4f26-bda6-4c2d52dc6e11",
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
              "id": "635795ae-f12f-452c-b405-1fb35d745bd3"
            }
          ]
        },
        {
          "id": "3c9aff03-8884-4c8e-ac72-c086c60c04ed",
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
              "id": "256e43a3-31be-4f18-99ed-04d6002896b9"
            }
          ]
        },
        {
          "id": "45d630ac-84c5-48f9-b0d6-9e043b497cbd",
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
              "id": "1b37c455-3b59-4214-afff-87cbfd93d07b"
            }
          ]
        },
        {
          "id": "02bf4f95-9fdd-437e-a99c-26b61936fda5",
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
              "id": "f2bcc6ac-1ba8-4f5a-83f6-1bdaf1e1913c"
            }
          ]
        },
        {
          "id": "71c2148d-1056-4873-9ff1-e81b4b824d39",
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
              "id": "553d8381-aa8e-48ab-9c95-f08bd125bec5"
            }
          ]
        },
        {
          "id": "f1e501c2-cc4f-4143-81cd-e5f0049c2590",
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
              "id": "92a9adfa-6270-446f-b072-121ffa730caf"
            }
          ]
        },
        {
          "id": "4a378f0a-a9ab-4d29-ae7d-1c1895682c82",
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
              "id": "74f9572b-8b86-4488-b72e-78ea955e2086"
            }
          ]
        },
        {
          "id": "69f44c46-e57d-42a6-b543-a5b66143ba83",
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
              "id": "efc0218e-3d49-47df-ab1d-83a2110a4113"
            }
          ]
        },
        {
          "id": "f6dc2576-6be2-4b5b-9480-32304b6a430c",
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
              "id": "32084d01-80f7-4948-ba3f-d96014ace67e"
            }
          ]
        },
        {
          "id": "8eabf992-649c-4ba5-957e-556eff686e25",
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
              "id": "12a2b49f-1688-4378-845b-6437b4ce77c1"
            }
          ]
        },
        {
          "id": "21365149-2d6c-44a9-9c15-507f826cf1d4",
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
              "id": "5345dd57-a7ed-4029-950a-dcff49902bac"
            }
          ]
        },
        {
          "id": "911fcfda-f304-48f9-a584-e0432bb7944d",
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
              "id": "281797dc-3669-4693-907a-93adfa35aacf"
            }
          ]
        },
        {
          "id": "4e4ddb7a-6e56-459c-8909-492f11bfc916",
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
              "id": "de4cd67e-1dba-4f5f-9176-239217570bdc"
            }
          ]
        },
        {
          "id": "499f24bd-dd73-4f4b-a873-72a396ba7110",
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
              "id": "ccfb6c6d-6f64-4482-9a11-a506aee7fd5f"
            }
          ]
        },
        {
          "id": "9b8d4afe-731d-44ae-af4d-4c3b6edd6ddb",
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
              "id": "9a9d393d-2286-40a4-9401-400639083b14"
            }
          ]
        },
        {
          "id": "5772ac27-9152-4837-9bd8-3f481b016477",
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
              "id": "05673270-42cb-4ee1-89c2-b480b4d65615"
            }
          ]
        },
        {
          "id": "29097164-b4cd-44f4-99ca-88f74faa3a72",
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
              "id": "b7a5a4aa-ebbb-444c-bb86-7a1398e3433f"
            }
          ]
        },
        {
          "id": "0200665e-87e2-4a8d-863f-5ddbfe8f00e8",
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
              "id": "c5a2d510-252b-4b7f-adbb-481666b48bce"
            }
          ]
        },
        {
          "id": "f66a71ac-564e-46aa-afa6-a82a0fa6ab4f",
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
              "id": "ac0b4442-198a-47ae-b69e-7d0c921ea091"
            }
          ]
        },
        {
          "id": "ccff7a2c-f92d-4354-98af-1dd86fa459d1",
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
              "id": "46f471ee-adfa-4f6a-bce7-2be39d1edea8"
            }
          ]
        },
        {
          "id": "da882e97-61af-4f7c-bc95-1b809ac3d4dc",
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
              "id": "2408629b-3f07-4266-bcfb-4abb665c7238"
            }
          ]
        },
        {
          "id": "e147457e-720d-41e0-b7cf-8a2c4757cb95",
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
              "id": "14090ad6-1f47-431f-ba1a-03aabb45b87e"
            }
          ]
        },
        {
          "id": "1d466caf-6526-421b-874e-19dc37ac997e",
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
              "id": "50aa62da-2149-43c9-a82c-6aca1133357c"
            }
          ]
        },
        {
          "id": "a9febf6e-5949-438a-b838-635dde11d3c6",
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
              "id": "c6c65216-6c18-4ddb-87ae-374dd8927463"
            }
          ]
        },
        {
          "id": "6f63ed32-319e-4a24-ba41-a7808df93072",
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
              "id": "5839be33-ec73-4fb7-a4b2-13df66b0d3cf"
            }
          ]
        },
        {
          "id": "563113f0-8de5-40f4-9ea5-276334fdeb17",
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
              "id": "104aa44e-dc67-46b3-b7e9-0e0698c6c09b"
            }
          ]
        },
        {
          "id": "afccfee3-5aa8-48cc-995a-940d2491f832",
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
              "id": "d8e0d0ee-c365-484a-8502-6eea64e04020"
            }
          ]
        },
        {
          "id": "6a33a524-f36d-4f4d-901b-ff115e8a6795",
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
              "id": "8cd73c87-297f-48b0-95a2-ca9d13a8e56e"
            }
          ]
        },
        {
          "id": "56e928d9-a6a6-435d-a9e1-15b6151d808d",
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
              "id": "29b5033f-78ca-4843-9a1d-13cce318fd1b"
            }
          ]
        },
        {
          "id": "f464faae-3957-4455-a7a2-8d02ce76ffd5",
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
              "id": "2a4bffc5-9895-4234-ba68-6e56bd428f39"
            }
          ]
        },
        {
          "id": "55ef158f-8612-44fa-afec-bfb0ff1b7bce",
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
              "id": "6d11e7d5-dd8e-4831-a539-d6495edb0d8f"
            }
          ]
        },
        {
          "id": "0892e20b-de65-4f7e-9e1a-e5776c4a7e18",
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
              "id": "80db8628-9206-4c53-9745-f406ce951213"
            }
          ]
        },
        {
          "id": "aecf75c9-c18b-4f58-b271-71f98b39377a",
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
              "id": "493ef474-acf3-46ea-9ae6-43d1e960e3be"
            }
          ]
        },
        {
          "id": "7c2f5754-a388-4262-8042-1d4031c57a94",
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
              "id": "47d8edf0-bb32-478d-b1e5-914bfac096bf"
            }
          ]
        },
        {
          "id": "7dc805c2-a1fd-4d50-9300-5c6292cf0ddb",
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
              "id": "08977be8-2d26-4c31-b21d-da7b57a5baf2"
            }
          ]
        },
        {
          "id": "cc11e92d-1078-4f87-8692-a40c628e109a",
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
              "id": "e2f049f9-8406-4ec1-bdf7-5d45ee7b4d5b"
            }
          ]
        },
        {
          "id": "1bf9edca-0563-47cf-a6d8-0b85df0f0b0d",
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
              "id": "2daf0682-3b62-4b59-8dfe-45de2e330136"
            }
          ]
        },
        {
          "id": "0c9bacc8-310b-4d82-93be-e54686fb92c4",
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
              "id": "6ee0ba02-8776-4344-98ff-fd50f7ce5b53"
            }
          ]
        },
        {
          "id": "9645372b-748d-4a29-b3f9-a6a7157995af",
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
              "id": "88931603-d04f-4a68-a21a-a76aaeb14bef"
            }
          ]
        },
        {
          "id": "d3558f35-5543-4426-9313-b772f991cec9",
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
              "id": "108a4259-3ef2-4521-90d0-5300435b684c"
            }
          ]
        },
        {
          "id": "ce6a1c92-3b3f-4be8-8322-06a63375802c",
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
              "id": "26e2b66d-4cbf-4ec7-a050-6a00a0d6a0a3"
            }
          ]
        },
        {
          "id": "00e88e9f-d5f6-4841-8980-f0c6efc3fe3c",
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
              "id": "118a44aa-cf76-4673-ae6e-03bff5db5c72"
            }
          ]
        },
        {
          "id": "2c7cadd5-5925-4feb-9b5d-9c6767bf80dc",
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
              "id": "4cb22a34-1642-436b-8017-14c7a8b983e1"
            }
          ]
        },
        {
          "id": "ea0044c6-528d-4b44-9c9a-f6693a4936be",
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
              "id": "94787afc-70d3-4c94-bca1-f673976a81fe"
            }
          ]
        },
        {
          "id": "4136f93f-31d1-4aef-917a-f059a7b824c4",
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
              "id": "93397303-e6c2-4797-b294-90f707e0a3a9"
            }
          ]
        },
        {
          "id": "95c91160-59c6-4bf7-9917-cf5dfaf88e71",
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
              "id": "f49691e2-cb93-4c00-ba7b-d2fcf5132204"
            }
          ]
        },
        {
          "id": "3a6d8fde-1794-42e1-8379-9b840748a632",
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
              "id": "f8e1f224-94fb-4a21-96ba-39d45c44429a"
            }
          ]
        },
        {
          "id": "40b267a3-5b75-4e2d-b171-2e88f9a0036c",
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
              "id": "c3052317-3ce7-46d1-a59a-ad0af3fdc18a"
            }
          ]
        },
        {
          "id": "3ba233dc-2532-4499-91f7-4c868dfddb20",
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
              "id": "ec3ab426-03d0-491e-9360-06dcd22a63a1"
            }
          ]
        },
        {
          "id": "a31c22ec-b22b-484d-aaa5-49839dfde87f",
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
              "id": "0443455c-5b18-41f4-9c37-11d2a33f66d3"
            }
          ]
        },
        {
          "id": "8e26424a-c105-46d7-9656-c9d515133d67",
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
              "id": "b5ed1792-53e5-4396-865f-4950cb42085f"
            }
          ]
        },
        {
          "id": "4406ee6f-6d01-4d8f-b350-7abc28bf57a3",
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
              "id": "436fd559-af9a-474c-ae44-c5b33fd42d27"
            }
          ]
        },
        {
          "id": "ba97f9fb-c969-4e7c-bffc-141d24f77b22",
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
              "id": "130a6ac8-3936-4772-a16c-14ffd496351e"
            }
          ]
        },
        {
          "id": "5654b9de-1858-4304-9499-5288eb7022ef",
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
              "id": "f1fd8b49-c3dd-4862-affa-cfadd590a4b7"
            }
          ]
        },
        {
          "id": "c3900aa9-d5c6-49f7-b798-225144e7a058",
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
              "id": "ead15a2d-5923-4919-8280-3eb27b804cb8"
            }
          ]
        },
        {
          "id": "7ee10e2b-3b04-4543-a697-332b2521ebcf",
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
              "id": "5d9fc233-193b-437a-94e3-160ee824b7ff"
            }
          ]
        },
        {
          "id": "fb65642b-f2bf-4df4-9513-39bb9de28a3c",
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
              "id": "0867f626-cf13-4841-85e4-7f99ba59b141"
            }
          ]
        },
        {
          "id": "789346e0-07d3-4187-9afe-24eed8f9c54c",
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
              "id": "de82d4e1-3231-4bfb-bb65-17ecf3cc60a5"
            }
          ]
        },
        {
          "id": "43e66614-15fc-4d09-9dae-57c5711ab519",
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
              "id": "b03d338a-5762-4cdb-a88d-e9e247f6287c"
            }
          ]
        },
        {
          "id": "353e607f-cf78-42c8-b3b0-fef43e6a5185",
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
              "id": "289cc19f-c64a-49c2-b7fc-b61f3f786cd6"
            }
          ]
        },
        {
          "id": "25170537-5806-4169-8730-7b56a9621ba4",
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
              "id": "fcefc4bb-0018-4e76-9816-f9a576a9340b"
            }
          ]
        },
        {
          "id": "f2af7ce2-eef7-49ed-bae4-7b6cda0959b2",
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
              "id": "73e1620e-51d3-48d4-bc41-06783a8f57ab"
            }
          ]
        },
        {
          "id": "482d55ad-f4b7-45cc-8987-042d0a13e539",
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
              "id": "946a617e-6a4c-4abb-9f62-5847890032f7"
            }
          ]
        },
        {
          "id": "a699a294-2ba6-49e5-8ae5-52a4a7aba37d",
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
              "id": "d9942f85-877f-4131-a9f2-f0b6869ba2a4"
            }
          ]
        },
        {
          "id": "89ee3010-5eed-4f63-b58b-5096823e60e9",
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
              "id": "3516efc9-a008-4ed0-b052-6bbaf79b84fc"
            }
          ]
        },
        {
          "id": "ee999350-12b0-4b28-a2a2-25782eb83f04",
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
              "id": "3db6e24d-d647-477a-8c48-025f439f699f"
            }
          ]
        },
        {
          "id": "dfafc5d4-0396-407f-b78f-efe5221b1c1f",
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
              "id": "5ce29db9-af49-47b1-b4b1-8bc8c3fc0409"
            }
          ]
        },
        {
          "id": "98f1778a-62b5-4599-a4be-0f604fc80fbe",
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
              "id": "3ef9950c-b204-429a-bf31-0a29728f76ff"
            }
          ]
        },
        {
          "id": "6641dd04-e861-434b-851b-76c2382a55ee",
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
              "id": "f321de78-a08a-4093-88f6-60b895f1e7f5"
            }
          ]
        },
        {
          "id": "e5ed1ed1-ecd5-48e4-bbf9-c198dc100c4d",
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
              "id": "f6a8e693-04cd-41f1-b887-a006d7fe7b3e"
            }
          ]
        },
        {
          "id": "123b545f-ad1d-4930-8f33-d2bbc54ebb8a",
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
              "id": "948e5d32-7c9e-4787-81df-91e53b255ff1"
            }
          ]
        },
        {
          "id": "aa9bda4c-6601-4d3e-a7e7-046fdfb64fc5",
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
              "id": "d524fd56-8a88-48d6-853e-db84149bf24a"
            }
          ]
        },
        {
          "id": "dfcf87a4-e264-44f0-89bd-9a745dc63203",
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
              "id": "9704ae69-42ca-4b4c-b507-51dbd66102a0"
            }
          ]
        },
        {
          "id": "7a5b2186-d6a0-445d-82e3-ed0c691069b7",
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
              "id": "146e93ef-ef19-443f-ada9-b66b44a098fc"
            }
          ]
        },
        {
          "id": "2635f5da-8c56-4314-98b1-2dcde4cfef25",
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
              "id": "b7ec2a16-646b-464e-9bb9-ab9200806d15"
            }
          ]
        },
        {
          "id": "8777dcea-50b0-4104-a113-79877ca4da62",
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
              "id": "76d54b82-a25a-4988-b7b1-0ce0b0628892"
            }
          ]
        },
        {
          "id": "8ccf9313-8025-4a32-951f-aae59617b17c",
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
              "id": "0834044c-f952-41e2-b1d7-68ede6a5f88f"
            }
          ]
        },
        {
          "id": "16ed1443-a647-4336-84fb-c02dea62a562",
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
              "id": "4127d20f-c39c-4b09-af19-93461fc55382"
            }
          ]
        },
        {
          "id": "560dbf32-bcd9-4ee7-9e05-f13cb8461fd6",
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
              "id": "babb2338-1d85-40ed-afed-8ce31382193e"
            }
          ]
        },
        {
          "id": "eb09f429-71b4-4c6b-b07c-1cc09b03e98b",
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
              "id": "691ce866-af5d-465c-9019-f30f5582d964"
            }
          ]
        },
        {
          "id": "8508e9a7-d15d-47a9-a1e4-034dda03ee1e",
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
              "id": "b20d5403-b37b-429d-aed2-ef3ca94c0322"
            }
          ]
        },
        {
          "id": "1a12caf3-be64-44db-85d4-12ee5adf9b7d",
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
              "id": "518e37fd-dc13-4af2-8ced-7ac2d3a65b0a"
            }
          ]
        },
        {
          "id": "bb547bc3-c972-41c7-8087-62ef8758c53f",
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
              "id": "d31b1eb7-b734-4c1f-8fed-0593c045ffb3"
            }
          ]
        },
        {
          "id": "4a703195-b89a-4be1-9abc-49b41be1a0d2",
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
              "id": "dfc87ac7-a234-45b3-a8eb-ad056d935e41"
            }
          ]
        },
        {
          "id": "5fc0eaa2-68bb-4966-8939-0a6b779c8c20",
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
              "id": "d718df33-f7f6-4ea3-975c-35cbe51d508c"
            }
          ]
        },
        {
          "id": "a66f1a66-eb78-4d6a-a79d-84d9819f0ad8",
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
              "id": "18792ac3-563d-4f96-a971-1331d0da4101"
            }
          ]
        },
        {
          "id": "a7e6efe5-7c7a-4132-b3c4-53951af2c5ce",
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
              "id": "1313fb87-4536-486b-9c80-60f31d51c44d"
            }
          ]
        },
        {
          "id": "27155fed-b631-44e2-bfa5-bb7588bb3f3f",
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
              "id": "c180ebd0-6e21-4697-b4e8-8f53430b9bd8"
            }
          ]
        },
        {
          "id": "258cbe4f-2117-4efa-b100-db9097484c52",
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
              "id": "291db585-8832-4498-bb43-43b382739134"
            }
          ]
        },
        {
          "id": "cd34821d-ca9b-42df-9dbe-d60c9697fb41",
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
              "id": "a602446e-70e5-4609-af3c-dc01c9223667"
            }
          ]
        },
        {
          "id": "af6d8a3b-5a46-412c-982c-74c865c99c20",
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
              "id": "b5aac73e-70cd-4c7d-a648-eee2dda521f1"
            }
          ]
        },
        {
          "id": "0f82309a-a0c4-433d-9810-d2cc18e865be",
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
              "id": "9910dfc1-9fd2-45dc-8a1e-67df0f2c2531"
            }
          ]
        },
        {
          "id": "13f7eb1e-e1a5-464a-83a1-62c172d55f9a",
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
              "id": "cfbb4acf-68ab-4456-8127-c1953b033ab8"
            }
          ]
        },
        {
          "id": "3bae62dd-8b7b-4380-b2f1-5ab398d5b4f8",
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
              "id": "22fbf8b2-9603-45b0-a71a-6326a22bb1a9"
            }
          ]
        },
        {
          "id": "1ed610ba-b1b2-454f-8a55-e269f27323b8",
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
              "id": "2f510183-970d-4943-b756-c3ec842e4284"
            }
          ]
        },
        {
          "id": "6d515057-28e8-47d1-a04c-7cbf0d614668",
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
              "id": "0b7a14fc-9ccd-41fb-8168-9318722d44a3"
            }
          ]
        },
        {
          "id": "098ad5ce-5a47-4aac-a618-08a3455b84d1",
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
              "id": "ef18a2f0-d04d-41bc-aae4-2172ed620d64"
            }
          ]
        },
        {
          "id": "e839258b-b4c9-4fd3-898c-6caa0e4d4da0",
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
              "id": "fd6e8458-7350-420e-bbe1-d6f61755462f"
            }
          ]
        },
        {
          "id": "ec260d0c-3b1a-41f6-85fb-9128ee5342b8",
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
              "id": "9e8d6be0-99ef-4af4-98c2-b57d723121b9"
            }
          ]
        },
        {
          "id": "3e773d57-af5d-4a58-9deb-725a492eed58",
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
              "id": "20969644-019b-46fe-a72c-df73ecebb1cb"
            }
          ]
        },
        {
          "id": "b5a714e9-f9bb-4fd1-b06b-4a9a6d01a1f1",
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
              "id": "ef19aca3-2544-4861-9ae4-8ac457c0f98e"
            }
          ]
        },
        {
          "id": "97880d79-e429-425d-b4f9-0a394a77898b",
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
              "id": "e80bd401-a579-44ad-8b40-9b1a1beb34fb"
            }
          ]
        },
        {
          "id": "f374f418-3fbc-47ce-b639-e0c2183a2a0c",
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
              "id": "44bd4104-7e4d-4080-a3cf-00c75488e7d1"
            }
          ]
        },
        {
          "id": "4eb88267-a29b-4fc6-be57-dad519106b4a",
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
              "id": "89746617-fe11-4c87-bdaa-315f4c5615f1"
            }
          ]
        },
        {
          "id": "118a2955-718b-47a9-9bd7-b8ccc46f0cf7",
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
              "id": "4fb6bfc9-1fdd-450c-afb1-b6121e8e2f3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizationss",
      "item": [
        {
          "id": "91645a14-7cf8-4ccf-9911-0e36c9934881",
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
              "id": "58a5168a-4619-4874-aaac-e32faf0efa5f"
            }
          ]
        },
        {
          "id": "1a1abbcf-b366-4da4-b68c-dde6dda45053",
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
              "id": "50eff8d4-ef3f-4c97-8dba-8b86f826c98f"
            }
          ]
        },
        {
          "id": "87460fc8-71a3-4621-bf15-51a52be8a1a6",
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
              "id": "9598473c-4dfe-4fd3-b1ba-76c71f2c64d3"
            }
          ]
        },
        {
          "id": "a919e2be-eb85-4d57-8694-4da758bf315f",
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
              "id": "4d006712-d3bb-4140-83f2-73904e1d1736"
            }
          ]
        },
        {
          "id": "fd0ece8f-9f67-40ac-a2de-ce1ed37af3c8",
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
              "id": "aaf70826-50fb-4f44-a9cd-e45811a2359c"
            }
          ]
        },
        {
          "id": "22abac54-c208-4984-91b8-b60abd9bed2c",
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
              "id": "a8a8f2f5-7472-4cfb-80da-d09f6eefef22"
            }
          ]
        },
        {
          "id": "93f8df76-1f2e-4ccd-951c-c315e9ef5923",
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
              "id": "fa9e33d4-8472-40e1-ae3a-499c225830b6"
            }
          ]
        },
        {
          "id": "1923e55c-2e28-48db-9309-fdffafbc85db",
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
              "id": "15b01a44-e3b4-4215-ac6d-d71f4bb43513"
            }
          ]
        }
      ]
    },
    {
      "name": "Auditsanizations",
      "item": [
        {
          "id": "142f198c-5c95-49d3-a150-0cc32a7f8653",
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
              "id": "61c3c70d-36c3-4aaf-97e1-85dad60be3cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "107aee56-6520-45f2-9a63-cb916befd540",
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
              "id": "4c833055-39fe-489d-aa2e-d88b5c8c04f7"
            }
          ]
        }
      ]
    }
  ]
}