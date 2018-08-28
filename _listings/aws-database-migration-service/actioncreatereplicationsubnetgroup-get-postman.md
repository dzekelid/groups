{
  "info": {
    "name": "AWS Database Migration Service API Create Replication Subnet Group",
    "_postman_id": "4fa26226-5a48-4384-bcfa-215df3e34d51",
    "description": "Creates a replication subnet group given a list of the subnet IDs in a VPC.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "cdfa26cd-bb30-4160-9d48-ea098d6999b0",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceArn=ResourceArn&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to a DMS resource, including replication instance, endpoint, security group, and migration task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "350830e0-1461-473e-8af0-1e28faa2f04f"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "365aef70-47dc-4e9f-bb04-b417cc326c6f",
          "name": "createEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreateEndpoint?CertificateArn=CertificateArn&DatabaseName=DatabaseName&EndpointIdentifier=EndpointIdentifier&EndpointType=EndpointType&EngineName=EngineName&ExtraConnectionAttributes=ExtraConnectionAttributes&KmsKeyId=KmsKeyId&Password=Password&Port=Port&ServerName=ServerName&SslMode=SslMode&Tags=Tags&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint using the provided settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "423b2a89-f5b9-4752-9eab-8251880d949f"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Instances",
      "item": [
        {
          "id": "5d16400b-e57d-45a0-bc1b-4902dcf796e0",
          "name": "createReplicationInstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MultiAZ=MultiAZ&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PubliclyAccessible=PubliclyAccessible&ReplicationInstanceClass=ReplicationInstanceClass&ReplicationInstanceIdentifier=ReplicationInstanceIdentifier&ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier&Tags=Tags&VpcSecurityGroupIds=VpcSecurityGroupIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the replication instance using the specified parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b458893-37f4-4fe1-8bfc-6f12fe9ad194"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Subnet Group",
      "item": [
        {
          "id": "20db114a-188c-427f-a55f-53eac8da9504",
          "name": "createReplicationSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationSubnetGroup?ReplicationSubnetGroupDescription=ReplicationSubnetGroupDescription&ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier&SubnetIds=SubnetIds&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a replication subnet group given a list of the subnet IDs in a VPC."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9dd1f46-0ca6-4e53-a976-56505cad583d"
            }
          ]
        }
      ]
    }
  ]
}