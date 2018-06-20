{
  "info": {
    "name": "Apigee Edge Delete Userroles Role Name",
    "_postman_id": "6492258c-4b86-4ac0-92a7-9c44ff20e134",
    "description": "Deletes a role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "0e772b84-e749-419c-9157-c382563ab458",
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
              "id": "fcb45b05-71f4-45c1-ba40-704a2b97679d"
            }
          ]
        },
        {
          "id": "f4f983d1-dc1d-4da5-bdda-b6f976eb8644",
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
              "id": "c7057e1f-d363-4363-8dc0-ace3fdd2a30d"
            }
          ]
        },
        {
          "id": "ed6cb523-1ccd-47f5-b0ed-fbc323cd9eaf",
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
              "id": "86f15174-b5cc-4248-b1e8-8564424098d8"
            }
          ]
        },
        {
          "id": "43c732bd-1a0e-46a0-b4ca-d4a9d3d40bac",
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
              "id": "de27de65-0667-4bfe-b637-9f7b2d6a352c"
            }
          ]
        },
        {
          "id": "c06d7654-d4be-4932-876d-9f2cc94331bc",
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
              "id": "9919706a-206b-430e-97f0-830684afc39a"
            }
          ]
        },
        {
          "id": "12e9ae83-0a90-45f5-8e45-154cb7c97a0a",
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
              "id": "77d3b25e-1711-4e1f-9d38-7067034b7398"
            }
          ]
        },
        {
          "id": "d8b6c460-8603-43f5-b2e0-8b42f6b3256a",
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
              "id": "24e3583b-2a39-42fe-b9c7-c05e3b2da4c5"
            }
          ]
        },
        {
          "id": "3db2a557-4f4d-4962-89cf-f5f669686831",
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
              "id": "b5c1daa4-9adc-47cc-8d83-575809d115b0"
            }
          ]
        },
        {
          "id": "be56eb3d-1b8d-4a58-9b1c-3954519fb225",
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
              "id": "e14d0c3f-4f56-4b87-aade-b37b7f73963e"
            }
          ]
        },
        {
          "id": "2b4af38c-6989-4d54-9fc5-2122d9d3b868",
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
              "id": "c7c0d0a7-d894-43f2-96cf-479955c36948"
            }
          ]
        },
        {
          "id": "c98a9213-cbc6-43c2-9aa4-5b2e4b530f8c",
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
              "id": "ada0a1d0-a111-4ae2-8242-cd688a955ec6"
            }
          ]
        },
        {
          "id": "4419f914-285a-413a-b323-5558443fa66d",
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
              "id": "efab1bae-0904-47ef-b5ef-b5d0c9a7c17f"
            }
          ]
        },
        {
          "id": "a9af566a-daf1-4e9c-8c08-cc4bca7fdf00",
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
              "id": "612e8fb0-f67a-44ec-9ddd-5a75726c1b6e"
            }
          ]
        },
        {
          "id": "a7df15bf-7661-4cd1-ae90-cb0faa985b70",
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
              "id": "72fcfe1e-3152-4f46-896c-01ea3d807e1a"
            }
          ]
        },
        {
          "id": "b100d331-71d2-455b-bc35-52296b24cb19",
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
              "id": "a6edebf5-7c02-4338-a320-90fff6b886e1"
            }
          ]
        },
        {
          "id": "e424e74d-c4c3-4821-986f-827b8e216a76",
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
              "id": "edf03769-85a3-4946-94b3-82331a226e0f"
            }
          ]
        },
        {
          "id": "7e5db9a9-3613-4be9-8c23-2ee79d9fbc89",
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
              "id": "cd6246aa-5157-4ac2-9aaf-3bd64cd550db"
            }
          ]
        },
        {
          "id": "5f2e3ed6-2b4e-4ce9-9f83-79c06787bd68",
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
              "id": "61fd0f3c-0094-40be-8b69-cb6984d3033e"
            }
          ]
        },
        {
          "id": "9e8dcea8-1e38-4483-bfe8-ef41043f8c9a",
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
              "id": "bef39a9e-bdce-4554-9c54-a61188c6c5a2"
            }
          ]
        },
        {
          "id": "1847ce78-6fad-455a-b4e3-5714972eb239",
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
              "id": "c128efc8-db9d-4cf5-ae69-3bf277da3ac2"
            }
          ]
        },
        {
          "id": "028110d9-ecdc-4394-99f5-78c9c7df29b7",
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
              "id": "60e4db1c-bfda-49ce-b7f9-efb687f50484"
            }
          ]
        },
        {
          "id": "1d16d01d-7a52-41f4-8995-4ed94c2a4406",
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
              "id": "c05b934e-78cb-4260-9dc2-b6667709c9b9"
            }
          ]
        },
        {
          "id": "be8842aa-7ad5-4623-9dbc-fe13e406917e",
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
              "id": "806c7fef-588a-4dfd-9823-0b20fc6ccb17"
            }
          ]
        },
        {
          "id": "34125ce3-dbe5-4215-ada1-e0510f77bd0d",
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
              "id": "48c0fcae-23cc-4c69-aa0f-1a4d9b599712"
            }
          ]
        },
        {
          "id": "48a6c25e-7579-4566-87c4-729e2f4f0f09",
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
              "id": "b2dff3d2-7f84-4ab5-84c7-d9fad474c724"
            }
          ]
        },
        {
          "id": "a28b9738-5387-48f2-87c2-10cd9a7a992d",
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
              "id": "e48fed2d-6efa-4087-8f4b-d2868818a534"
            }
          ]
        },
        {
          "id": "6a08c33a-5803-4801-bd9e-ee46a7c8320e",
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
              "id": "42afdb25-b26a-4133-8576-0015d359c837"
            }
          ]
        },
        {
          "id": "481dba55-b82d-40b8-9b0e-7c358f4fe262",
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
              "id": "24f7b371-ca6c-4e12-ab5e-a78d1c1b043e"
            }
          ]
        },
        {
          "id": "3977ba17-21a4-4993-b529-27f87fa3cbbf",
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
              "id": "2f17c070-8ff8-4a10-a38a-bb83a76f2890"
            }
          ]
        },
        {
          "id": "40ce91b6-c68f-427c-aa76-2f6156707b59",
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
              "id": "b13916c6-c196-446f-b7ce-74214187d73a"
            }
          ]
        },
        {
          "id": "6cb8dc95-ec1e-412d-abb9-0fc58a1cb5a5",
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
              "id": "7b88af58-b906-4fe1-899c-3c18b97ec4f9"
            }
          ]
        },
        {
          "id": "c2c1a2f0-c042-4d43-9086-1ab75c1a80ff",
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
              "id": "4657ce91-2a62-444a-a792-01f6f643b7a5"
            }
          ]
        },
        {
          "id": "48237b66-7b46-4a16-b41c-0677b0d676cb",
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
              "id": "ca35a9ff-448c-43f2-8962-4b78bc67a276"
            }
          ]
        },
        {
          "id": "8d383e33-f3c3-4d88-908b-77460df8418c",
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
              "id": "a054aafe-c88a-4457-8383-54ac83017a5d"
            }
          ]
        },
        {
          "id": "2c572b1f-d979-443d-99cc-3369dbd43b57",
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
              "id": "4df825e6-7e53-4b35-a0a8-973845b7c4dd"
            }
          ]
        },
        {
          "id": "e19c73ba-3d60-49e2-8150-33091b3a01ea",
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
              "id": "1c360a76-4b75-4a72-8841-9505857def61"
            }
          ]
        },
        {
          "id": "dbcf3503-7392-44cf-85e2-ea098a6256e6",
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
              "id": "5e5bc4d7-e916-40f8-bdb7-94fb1529ace3"
            }
          ]
        },
        {
          "id": "d088a68b-855f-48e7-8d9c-6923b3679e4b",
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
              "id": "cb539f18-16d0-429d-bbd9-36f47bb43d00"
            }
          ]
        },
        {
          "id": "f8d0e4f7-c0a8-4927-a788-698582549d67",
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
              "id": "b87153a6-8362-45fd-bce4-747412156666"
            }
          ]
        },
        {
          "id": "c9325bc3-5624-4127-bc23-7bf5ad7aee34",
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
              "id": "b200abe4-a283-4d88-8f4f-0cd4dadecc54"
            }
          ]
        },
        {
          "id": "854cdfd8-ea08-4bce-9b58-61fc88de38f0",
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
              "id": "d2368342-9633-4c3f-84ea-888e40df2462"
            }
          ]
        },
        {
          "id": "f4b2462b-7eaa-43c3-91f1-2d9ee6dafada",
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
              "id": "02effb1c-af93-4fd0-947c-d5e4460cf848"
            }
          ]
        },
        {
          "id": "f9cce6b9-a5c9-4f81-ab51-39f6cfebdd01",
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
              "id": "ace78f0a-9da2-4293-87da-e570aa433a46"
            }
          ]
        },
        {
          "id": "257b5bce-a34e-415f-9aa0-bf3d9678c35f",
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
              "id": "ec36f924-4bc5-4775-8708-045aae1a9399"
            }
          ]
        },
        {
          "id": "2b896d52-c4f2-4b01-8ef9-390eb30a7dea",
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
              "id": "7b17e296-ba46-4841-b122-d3d4d03ffa83"
            }
          ]
        },
        {
          "id": "e81ec967-6e29-4374-af2e-5baeccdf1808",
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
              "id": "95a93483-903c-4d02-94dd-7a7660d81e47"
            }
          ]
        },
        {
          "id": "2828ab45-9e9f-428f-aa49-d800b5021edc",
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
              "id": "6e8f5fcf-c2e5-4553-a50e-463b725debd1"
            }
          ]
        },
        {
          "id": "33187c2c-44d2-41a9-be54-050c5baf4109",
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
              "id": "fb3cc3c9-fae5-4f19-aebb-cd2c5a8945d0"
            }
          ]
        },
        {
          "id": "c7a851a5-616b-4f6e-9050-7365cbab7709",
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
              "id": "a614bc1d-a07e-4545-aa1f-b01555df9fd3"
            }
          ]
        },
        {
          "id": "c391fc78-fc21-4d0d-be3a-09a4fff41603",
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
              "id": "6c784a5d-50d7-4a48-b885-f307148ca327"
            }
          ]
        },
        {
          "id": "13c45bbd-973a-4aab-b95d-31dad3eb6988",
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
              "id": "d03ad2b1-c1e5-47bf-b1fc-3040e62c43e6"
            }
          ]
        },
        {
          "id": "b2c9f373-7711-4986-8e67-91f7f62ef29c",
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
              "id": "ad009a19-7f8f-4cd3-83ac-c1bf7131bfda"
            }
          ]
        },
        {
          "id": "2c0448dc-972c-4b68-80e9-3210997e886b",
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
              "id": "41d4c233-96c9-484d-9ce6-d9c8a43a0757"
            }
          ]
        },
        {
          "id": "4331b061-7140-40a4-9250-bcca8f121d28",
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
              "id": "5e052d09-fc5a-4937-bc10-9389d02a915e"
            }
          ]
        },
        {
          "id": "61e26ddc-c3e0-43cb-8879-0f13c6803859",
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
              "id": "6c6c53ba-3a06-4a2e-8a85-70be1b571a06"
            }
          ]
        },
        {
          "id": "ae4c2f46-ccbf-4d51-bf20-aad2e1bdaef1",
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
              "id": "fd5df3ec-19eb-4e98-bb0a-9e65b48b8a3e"
            }
          ]
        },
        {
          "id": "bb457a6b-21e8-49af-9c3d-63e17c2b2da9",
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
              "id": "cac54969-cc29-4703-92d6-9a13a262bbd5"
            }
          ]
        },
        {
          "id": "1d80e55c-ec5f-460a-80ec-cf69925100d7",
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
              "id": "b52ec303-56d7-44be-a71d-33eac9cf49fd"
            }
          ]
        },
        {
          "id": "8c55eb0c-94a4-4adf-858c-03b04dbcc99d",
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
              "id": "f726d6bb-f989-4d54-b254-3ba3dbc293ef"
            }
          ]
        },
        {
          "id": "6ac3bdfa-28c9-482f-b121-a0c08231043e",
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
              "id": "1037e529-958b-4222-9068-9f247a2ffe6e"
            }
          ]
        },
        {
          "id": "5f7a4356-ba9b-4a30-bdf8-013f2b6772a7",
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
              "id": "35f749d0-49c6-434a-a623-1f3adec65cb7"
            }
          ]
        },
        {
          "id": "b1be2212-de0d-4906-8526-f0c910e0ba51",
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
              "id": "089496b2-e089-429c-8133-f158e4b88e15"
            }
          ]
        },
        {
          "id": "73b891f7-3408-4ffa-8a8f-5def8390c6f4",
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
              "id": "90642544-1962-4a39-9040-3eee9d465017"
            }
          ]
        },
        {
          "id": "62a7e3a9-6b0f-4099-8645-7e975718e02a",
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
              "id": "19f2720f-a4b0-49ee-b0b5-56ff62b25796"
            }
          ]
        },
        {
          "id": "fbd48d5f-04b7-42df-84c6-7ff15809d0b2",
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
              "id": "e8a4d2c3-84fd-4adf-97c9-63b37e8f04de"
            }
          ]
        },
        {
          "id": "69b31139-7d45-4c88-a2dd-d8fb6c13575c",
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
              "id": "ddc36c88-03ac-49f4-ad3c-3aa72bc03bea"
            }
          ]
        },
        {
          "id": "19c882d9-7c2f-4fa9-b302-8ae27e11e4f1",
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
              "id": "3a0c4575-3619-4d46-b4b8-c4e87be15087"
            }
          ]
        },
        {
          "id": "855f930a-184e-4cd8-bcd3-eff8686e62ab",
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
              "id": "42bd5c7e-5bd7-4273-b2f5-f8985c10469a"
            }
          ]
        },
        {
          "id": "9ee61496-2e40-4e18-95e2-8a091911d408",
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
              "id": "8077269a-18ea-4c88-9d3f-4650e74fe246"
            }
          ]
        },
        {
          "id": "be1c386f-16cd-4620-b70d-ee41f6d738d9",
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
              "id": "b96c8f28-1dc8-448a-a3cb-941150600e5a"
            }
          ]
        },
        {
          "id": "973e18e3-a3ca-49dd-a768-e11b9ed5b379",
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
              "id": "64a6df89-0f6d-42e0-bff7-37dae730ea6f"
            }
          ]
        },
        {
          "id": "361d3c14-c261-4244-88cc-407928365e8d",
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
              "id": "d308c89c-77e1-4b96-a256-3b3e11a3918f"
            }
          ]
        },
        {
          "id": "ecc4d6a7-f8f6-4585-868c-5ccc3c35df82",
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
              "id": "7d6a3e3c-f26b-48c8-b0e9-86e10b2e3cf3"
            }
          ]
        },
        {
          "id": "4ff1efb6-e9db-4e08-b4bc-cdd9b6f52a83",
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
              "id": "cbea007b-f3c1-4161-b30e-551afd09d2ea"
            }
          ]
        },
        {
          "id": "b5a04db3-b81f-47ad-abaa-fd07adf93277",
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
              "id": "7b3c718f-e291-4131-a076-6fbd8960943c"
            }
          ]
        },
        {
          "id": "1fdc6309-6873-40af-8c7f-7df0d1c4b54c",
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
              "id": "c8d65498-3009-4639-8759-0c36e14bd188"
            }
          ]
        },
        {
          "id": "842cf32c-5201-4ac4-a972-8d605445394c",
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
              "id": "692b252b-b413-4e76-8136-22a630a47dc7"
            }
          ]
        },
        {
          "id": "e9423969-66a5-4536-9d07-e6aa90fb7e2b",
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
              "id": "028e49ed-017d-42c0-9c12-0de4bfcfc814"
            }
          ]
        },
        {
          "id": "c344a185-de07-49b6-818b-fe1366832db8",
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
              "id": "39e180d0-7d05-416b-9bf4-4b63c88cac13"
            }
          ]
        },
        {
          "id": "91b15390-b7c8-47b2-935d-34ad1c533018",
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
              "id": "b066cbc3-ed06-47fb-81be-04c4dbaf9d26"
            }
          ]
        },
        {
          "id": "7fd390e0-3a05-42f8-b8d9-28c79f7ef4f6",
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
              "id": "a59274c8-fb22-407d-a1f8-19c3b2b23565"
            }
          ]
        },
        {
          "id": "6bb19c83-794b-4ee9-8299-2a77f4318cc5",
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
              "id": "411c2bf0-c3c3-47a6-b5d8-d50f3250de7e"
            }
          ]
        },
        {
          "id": "d472bdc6-5116-49bf-a46c-0e1da80cfcb0",
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
              "id": "fc16f207-ec06-48a0-a2a2-d313be2e3ac5"
            }
          ]
        },
        {
          "id": "d67cc6e2-9c45-4ef0-ae70-04ada689c59d",
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
              "id": "bc94dc77-d202-46eb-a5ee-9ae69ba7e6c5"
            }
          ]
        },
        {
          "id": "b9c1c3e1-df59-40b9-a20b-a3d8c94e2d94",
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
              "id": "37a539ba-d359-47bf-9922-4ba35245a91b"
            }
          ]
        },
        {
          "id": "99a1372f-3acf-4c3e-ae7d-888c51378118",
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
              "id": "2cc4a907-4a49-48e2-8b47-e0678b693c34"
            }
          ]
        },
        {
          "id": "432133fb-d1a5-4794-b21e-39101ae4dba0",
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
              "id": "aa7cd30f-134e-40a8-a82b-866fc5b75277"
            }
          ]
        },
        {
          "id": "9cbcb4f2-2ce2-4bd3-9dd1-ea23ba72729c",
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
              "id": "e7e2d6f9-6ff4-4b5d-9c91-b4ad8b354475"
            }
          ]
        },
        {
          "id": "7b246295-79b9-4bff-8f7a-8abb95df258e",
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
              "id": "11704137-4a56-435f-bd70-20e7e7d17cc5"
            }
          ]
        },
        {
          "id": "209541d1-383e-49e7-9fe6-919a22473758",
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
              "id": "ff50919a-2f30-4d58-b5aa-92d933b00095"
            }
          ]
        },
        {
          "id": "9bc6fa6d-c109-4bc7-bbbf-c858a3567fd2",
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
              "id": "18321b87-d86d-46a4-95ef-dd92cdff8524"
            }
          ]
        },
        {
          "id": "d4417e45-1434-436e-85a6-2af995ac1f42",
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
              "id": "d92eaa37-ee78-41d6-8927-45f4d2cccc27"
            }
          ]
        },
        {
          "id": "18b9001b-9b23-4da7-bbca-5558b062dc08",
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
              "id": "9d7f01f3-4358-4bab-9626-1b506b77911d"
            }
          ]
        },
        {
          "id": "9dadbf17-a052-47aa-90ef-acfd2c51376d",
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
              "id": "277986ff-f27e-43de-b736-372610d12208"
            }
          ]
        },
        {
          "id": "93c9c505-69fc-4463-9f5b-8754e175074c",
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
              "id": "6edd362e-b676-40dc-8591-3120336354bf"
            }
          ]
        },
        {
          "id": "1fd431da-f980-4388-b5f0-406013829196",
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
              "id": "0343f942-7712-4f0c-afd5-2ab2cc9709aa"
            }
          ]
        },
        {
          "id": "047a6218-4586-4195-870d-566d4d7e53e7",
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
              "id": "37d7c766-1b78-4261-b321-11151aa17d58"
            }
          ]
        },
        {
          "id": "e385442d-7325-4bd4-bb40-43be972b8b8b",
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
              "id": "f7fa8965-df40-4977-beac-d64544bc4fe5"
            }
          ]
        },
        {
          "id": "83018c7e-e560-4203-8363-e67f6f95e91a",
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
              "id": "7ad92f72-7121-4638-afd2-eab1dd1d2fb6"
            }
          ]
        },
        {
          "id": "1011280a-f9d0-4549-bb2a-8335b22e0cc6",
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
              "id": "6c371763-d0df-4254-80da-2bfb682c4610"
            }
          ]
        },
        {
          "id": "007384de-fc80-4c4c-9521-afb0edb9c96d",
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
              "id": "71f32786-0d76-41c3-b7a7-8a990f7e21bb"
            }
          ]
        },
        {
          "id": "1d9b9c1e-95ef-4a81-aadf-80f909ea0104",
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
              "id": "5adadb36-1d1c-41c1-904a-e2982aa0224d"
            }
          ]
        },
        {
          "id": "b1a55b74-21b2-414b-89b8-f005ccf830bb",
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
              "id": "59519a4f-a056-4540-9989-71d95ba18200"
            }
          ]
        },
        {
          "id": "85fc2868-b57a-418b-9d77-425b34ce920e",
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
              "id": "e0dd0d0a-23e2-49cf-aaa8-38a475f99625"
            }
          ]
        },
        {
          "id": "307c8593-56b4-44f5-aa03-0ecc4ed2af6a",
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
              "id": "6890743e-f293-4c5b-a74c-e4b6e9344c61"
            }
          ]
        },
        {
          "id": "96fa8840-f0e0-4f24-bdb1-22000c30d7be",
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
              "id": "2ccea7eb-9de8-44f7-b27b-1510fbfcb0cb"
            }
          ]
        },
        {
          "id": "72570563-a873-4cba-b63c-9cecdf62003d",
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
              "id": "f5f5bf55-bb46-449e-8c02-15e2c1938179"
            }
          ]
        },
        {
          "id": "67a485b7-a308-4087-86d8-8d2eb9ceec66",
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
              "id": "1b54a5b8-862d-47ff-8680-870dceb55083"
            }
          ]
        },
        {
          "id": "3d308a36-690b-4dd8-abf8-ec6a0c6d47de",
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
              "id": "14e40937-3382-4bd3-a503-0c060e7fc77e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizationss",
      "item": [
        {
          "id": "50d44afe-1b65-456a-8b86-4a4e7c754ee0",
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
              "id": "1ed3950d-a9ee-4270-8fc8-35a7d8aa70f7"
            }
          ]
        },
        {
          "id": "34626dec-2ec5-49cd-8713-1e3687621706",
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
              "id": "179ca956-b885-44b8-aadf-702591e826d1"
            }
          ]
        },
        {
          "id": "673addf9-0e87-4a68-ac32-63bd43424924",
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
              "id": "9eb1d569-15b0-433a-a48c-7fcd1da1a967"
            }
          ]
        },
        {
          "id": "c6410bc5-6682-45b9-8ce3-a58261462db4",
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
              "id": "02ef7545-8ebc-4682-9c33-f76503043156"
            }
          ]
        },
        {
          "id": "c41ec1ce-3506-4e5e-ad00-c547be254ee1",
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
              "id": "01d51ef8-dc47-4c44-a2db-af65b8471943"
            }
          ]
        },
        {
          "id": "4d151f96-1509-429b-9ca3-9ec905985378",
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
              "id": "027a8530-d438-4c75-9ffa-790680c936f7"
            }
          ]
        },
        {
          "id": "20817da1-f2ac-4bd7-b41b-e3d05d7778e8",
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
              "id": "067d7a53-aff5-43b1-a6f2-adbc81db4ab4"
            }
          ]
        },
        {
          "id": "61d0414a-e12f-4bf8-8417-ccccdf5966df",
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
              "id": "5daf38d0-5e91-4602-87d3-f509a4be29e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Auditsanizations",
      "item": [
        {
          "id": "1ec89844-df2c-46ca-96b4-adbbe4bd6319",
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
              "id": "1ad49257-d2ad-4ce8-8541-a383e2c0a2ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "a79f00c5-dae8-472b-ae54-47e6537341b9",
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
              "id": "3e86038d-6bed-433d-9dec-5576b2138b69"
            }
          ]
        },
        {
          "id": "9e6ad264-93ac-4666-9e4f-a1081abe7cd1",
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
              "id": "d98720b2-8ef3-4724-b0da-5832ca53aa7d"
            }
          ]
        },
        {
          "id": "53868075-3236-4c7b-a743-f9d582986b90",
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
              "id": "5759750c-4f45-4b8a-b62f-3e6638df7b8d"
            }
          ]
        },
        {
          "id": "347bcff0-37af-4e9b-835e-d00c17139102",
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
              "id": "748399a7-a676-45b7-b284-d67f9e0fc3ef"
            }
          ]
        },
        {
          "id": "c847d2de-92b1-457f-b249-7f675569d508",
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
              "id": "6fdfe83c-37b1-49cb-8b83-5be73a07025f"
            }
          ]
        }
      ]
    },
    {
      "name": "Userroles",
      "item": [
        {
          "id": "7d3f17ca-bafa-4547-9dcd-6c9bb62e6647",
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
              "id": "e7246661-168d-4453-82c8-35d6d26a9920"
            }
          ]
        },
        {
          "id": "74a6cfc7-e329-44e7-86b1-caac0a85648a",
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
              "id": "ee369e77-95db-4056-907b-f0cfe63f6464"
            }
          ]
        },
        {
          "id": "4c6c9387-4d20-4b35-b51c-e503edf1b31c",
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
              "id": "4dc5c2b1-b369-495a-a04f-e104f1c56af8"
            }
          ]
        },
        {
          "id": "e41819c9-be46-4b66-818f-bd2a1338f0e6",
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
              "id": "b565786a-44f3-449a-b3ab-3380cda85de3"
            }
          ]
        }
      ]
    }
  ]
}