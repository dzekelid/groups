{
  "info": {
    "name": "AWS Database Migration Service API Delete Replication Subnet Group",
    "_postman_id": "160e8d20-2bbd-4353-855d-173cdf1d255c",
    "description": "Deletes a subnet group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "f2092151-bb59-4c9d-a989-524917a59022",
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
              "id": "b48c9f6e-1cd7-4d38-9535-87a1afa3674c"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "bb25ef01-26ae-4bef-a1a1-6b5263ebe8b7",
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
              "id": "82358853-5a4f-4a21-b96c-30acfdbc60c1"
            }
          ]
        },
        {
          "id": "6ceb44e7-7f06-42b3-b760-ca4990b3d9dd",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50ef7bc2-550f-4977-b8e4-0b04575b5032"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Instances",
      "item": [
        {
          "id": "b694450d-5fd3-4aaf-be35-a609f35868ea",
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
              "id": "18ae32b9-51df-4a3b-b7eb-5c3e0cdcc8c3"
            }
          ]
        },
        {
          "id": "43e145c5-adcc-4111-baec-b96c5f28e79b",
          "name": "deleteReplicationInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationInstance?ReplicationInstanceArn=ReplicationInstanceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified replication instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2378264-fdd6-487e-9aff-3a5eeb8cbf79"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Subnet Group",
      "item": [
        {
          "id": "f042428a-6c03-40b1-b048-3142eec30115",
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
              "id": "86027c71-3c30-4985-a81d-b68518dba034"
            }
          ]
        },
        {
          "id": "85ad86d5-2b28-4fd6-a864-e8bafc52a9e5",
          "name": "deleteReplicationSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationSubnetGroup?ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aba956ce-8274-4770-b1ce-0e898b5c9085"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Tasks",
      "item": [
        {
          "id": "fdf92cd0-3916-4161-bf27-73cba77fa6b3",
          "name": "createReplicationTask",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationTask?CdcStartTime=CdcStartTime&MigrationType=MigrationType&ReplicationInstanceArn=ReplicationInstanceArn&ReplicationTaskIdentifier=ReplicationTaskIdentifier&ReplicationTaskSettings=ReplicationTaskSettings&SourceEndpointArn=SourceEndpointArn&TableMappings=TableMappings&Tags=Tags&TargetEndpointArn=TargetEndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a replication task using the specified parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6af0a5f6-bc5a-44ac-911e-3531c16c00ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "6aa013e1-4cf2-47e1-a145-05cbfd7b69c4",
          "name": "deleteCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCertificate?CertificateArn=CertificateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f947bea1-02a3-4b5b-af53-f387d41c796b"
            }
          ]
        }
      ]
    }
  ]
}