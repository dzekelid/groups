{
  "info": {
    "name": "AWS Cognito API List Groups",
    "_postman_id": "82146ba6-93ed-4534-8aea-4beecc737380",
    "description": "Lists the groups associated with a user pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "2c99eab9-72bf-4a34-a602-5537e4c88a01",
          "name": "addCustomAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AddCustomAttributes?CustomAttributes=CustomAttributes&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds additional user attributes to the user pool schema."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9171a00b-a553-44a3-97ba-1ced8f46f4bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "76f0b15a-b0f9-4a6e-bc2e-ea65178426bc",
          "name": "adminAddUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminAddUserToGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e01abc7b-cda5-410a-8fea-042580af00bc"
            }
          ]
        },
        {
          "id": "78c03740-0463-4ca4-ad7b-da49d8b04c8c",
          "name": "adminCreateUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminCreateUser?DesiredDeliveryMediums=DesiredDeliveryMediums&ForceAliasCreation=ForceAliasCreation&MessageAction=MessageAction&TemporaryPassword=TemporaryPassword&UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId&ValidationData=ValidationData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user in the specified user pool and sends a welcome message via email\n            or phone (SMS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df2d60eb-ab54-4d57-9f25-d6c28afa1fca"
            }
          ]
        },
        {
          "id": "485bd2de-2b9e-4f60-9543-93044a244956",
          "name": "adminDeleteUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48161460-7453-46a7-92b0-d42ca84f4169"
            }
          ]
        },
        {
          "id": "f2f8a88d-58cb-4a39-8de7-77c21b4cf786",
          "name": "adminDeleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUserAttributes?UserAttributeNames=UserAttributeNames&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the user attributes in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4daa99a3-d04d-446d-93e0-9c5fd21d7742"
            }
          ]
        },
        {
          "id": "d115263a-f1aa-494c-82b3-6e74066f1343",
          "name": "adminDisableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDisableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bf03eeb-2ca2-49cc-bb1b-dfe60ae1f8f9"
            }
          ]
        },
        {
          "id": "f42a26d1-5a99-43c4-99f8-b7ecf6d8b391",
          "name": "adminEnableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminEnableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a057db7b-69b1-4520-b69e-f1840063b949"
            }
          ]
        },
        {
          "id": "2b5f0324-5ca9-48b3-afc6-5a2cb3e475a5",
          "name": "adminGetUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified user by user name in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39323de4-a4a2-4ada-8119-364bb67f8f48"
            }
          ]
        },
        {
          "id": "692ce572-0c38-4b84-9077-969fc0d4324f",
          "name": "adminListGroupsForUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminListGroupsForUser?Limit=Limit&NextToken=NextToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups that the user belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "145f2152-7fe0-480b-8633-ac6acfd04847"
            }
          ]
        },
        {
          "id": "c8a698c1-ebd2-4cfe-b277-f528d8e0bbf0",
          "name": "adminRemoveUserFromGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminRemoveUserFromGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified user from the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87f8574b-9fb5-4860-9c5b-f079863a01d5"
            }
          ]
        },
        {
          "id": "f03578e8-4e4b-4747-b193-bc036c69e324",
          "name": "adminResetUserPassword",
          "request": {
            "url": "http://example.com/api/?Action=AdminResetUserPassword?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resets the specified user's password in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d9b1b50-9cf6-4155-9a38-5a16cb3271c9"
            }
          ]
        },
        {
          "id": "d2f1d9c1-5b9c-4594-b2f0-05d7666513f6",
          "name": "adminSetUserSettings",
          "request": {
            "url": "http://example.com/api/?Action=AdminSetUserSettings?MFAOptions=MFAOptions&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets all the user settings for a specified user name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd1244fe-82fc-461f-a99b-d809de43918a"
            }
          ]
        },
        {
          "id": "5ac5275a-caa8-4874-9742-bd8f496a72d3",
          "name": "adminUpdateDeviceStatus",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateDeviceStatus?DeviceKey=DeviceKey&DeviceRememberedStatus=DeviceRememberedStatus&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the device status as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "951e00e1-802f-4c4f-8a34-80a01f41ecd2"
            }
          ]
        },
        {
          "id": "cfb86548-78c1-40aa-8490-534a264a39cc",
          "name": "adminUpdateUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateUserAttributes?UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified user's attributes, including developer attributes, as an\n            administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d668c7e2-d0a5-4178-b867-0acc2c946cb3"
            }
          ]
        },
        {
          "id": "be2042fc-a28a-4ecb-892a-83d3d64f5c25",
          "name": "adminUserGlobalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=AdminUserGlobalSignOut?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee5de360-4649-47e4-89d4-a7e9b1dca46a"
            }
          ]
        },
        {
          "id": "44730539-66bc-4e3d-8378-ca868332f6f1",
          "name": "createUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserImportJob?CloudWatchLogsRoleArn=CloudWatchLogsRoleArn&JobName=JobName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9298550c-21e5-476b-b92e-e3f5190c2147"
            }
          ]
        },
        {
          "id": "829237f4-107d-4bc9-b623-0fd342056390",
          "name": "createUserPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AliasAttributes=AliasAttributes&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&PoolName=PoolName&Schema=Schema&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Cognito user pool and sets the password policy for the\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c3c4faf-64d6-4ee0-b4e1-fcce5e274117"
            }
          ]
        },
        {
          "id": "2e1eecd4-2685-462b-9c7f-3dd679cc35d5",
          "name": "createUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPoolClient?ClientName=ClientName&ExplicitAuthFlows=ExplicitAuthFlows&GenerateSecret=GenerateSecret&ReadAttributes=ReadAttributes&RefreshTokenValidity=RefreshTokenValidity&UserPoolId=UserPoolId&WriteAttributes=WriteAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5b8de37-672d-4c41-ba77-56c3c25047a9"
            }
          ]
        },
        {
          "id": "3bf03469-053a-424c-8825-39fb1b00fe76",
          "name": "deleteUser",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to delete one's self."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a8592e9-e1b9-4b8e-b63c-27af2fe575d8"
            }
          ]
        },
        {
          "id": "2e37a435-e1a5-4854-94ad-3dd866a3daa9",
          "name": "deleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserAttributes?AccessToken=AccessToken&UserAttributeNames=UserAttributeNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the attributes for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd830cd9-15cb-47c8-9a0d-3f14badd6a2d"
            }
          ]
        },
        {
          "id": "ca09bcf3-26da-494f-8ec4-a35689255a97",
          "name": "deleteUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91cc018b-8849-4ae0-a912-e0b1fa074542"
            }
          ]
        },
        {
          "id": "ebf67a8b-e529-42d3-85ff-c0953ff92e0b",
          "name": "deleteUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to delete the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c157dc02-876f-4b03-aa0c-74a67c636ea4"
            }
          ]
        },
        {
          "id": "733daaf0-59da-420d-b934-480a1741bcfe",
          "name": "describeUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserImportJob?JobId=JobId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af905206-b76d-45fa-92f2-2476be2e69aa"
            }
          ]
        },
        {
          "id": "6b1024a2-cd22-4916-9e80-342e9b13a2f8",
          "name": "describeUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information and metadata of the specified user\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc1c9db9-8b82-40a5-964a-686bfdeca176"
            }
          ]
        },
        {
          "id": "fe378974-1e4e-423a-a748-b4fd1c0d6c09",
          "name": "describeUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Client method for returning the configuration information and metadata of the\n            specified user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d192215-f0bf-413f-aadd-fc74c99aae3c"
            }
          ]
        },
        {
          "id": "b1482d4a-6492-4474-89c1-9ac74c891529",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2e51091-12f0-41c6-8595-69715858aff2"
            }
          ]
        },
        {
          "id": "26a7f9ee-c49c-43ae-8353-43726864430c",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/?Action=GetUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attributes and metadata for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cff4ffe2-394a-441f-8f11-20d503da058e"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Up",
      "item": [
        {
          "id": "0d9bb853-3800-4b14-ad69-3bf43a6ad394",
          "name": "adminConfirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=AdminConfirmSignUp?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms user registration as an admin without using a confirmation code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c66e0fc2-7473-463d-a5f0-3106647e3e41"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "7dc90984-7f9d-4706-85b0-ef44dcebb02b",
          "name": "adminForgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminForgetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a2daf98-bb93-489b-8cf6-579644776dd7"
            }
          ]
        },
        {
          "id": "b345fbcb-3917-42eb-b248-eb8123c17a95",
          "name": "confirmDevice",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmDevice?AccessToken=AccessToken&DeviceKey=DeviceKey&DeviceName=DeviceName&DeviceSecretVerifierConfig=DeviceSecretVerifierConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms tracking of the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "459b9d4b-c22b-49a6-b3c0-c337c49765c0"
            }
          ]
        },
        {
          "id": "d08b08b5-a153-48b8-afa5-255d31d6ec91",
          "name": "forgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=ForgetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the specified device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2758075-457c-4503-8a6b-5baeb6ed28b0"
            }
          ]
        },
        {
          "id": "eaf91171-e868-4d75-b823-22dde175c0ba",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?AccessToken=AccessToken&Limit=Limit&PaginationToken=PaginationToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2580e48b-ac35-416c-9fb1-265ba5f58675"
            }
          ]
        }
      ]
    },
    {
      "name": "http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php",
      "item": [
        {
          "id": "14dca6e9-6f43-4caa-a3e4-6a72fbc16194",
          "name": "adminGetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56d60ba0-2917-40f1-9039-2ce52837aa80"
            }
          ]
        },
        {
          "id": "13fd6865-22ea-44ce-b312-407cb167c831",
          "name": "adminListDevices",
          "request": {
            "url": "http://example.com/api/?Action=AdminListDevices?Limit=Limit&PaginationToken=PaginationToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa54718c-9cef-45eb-9441-0317f46ba870"
            }
          ]
        }
      ]
    },
    {
      "name": "Authnetication",
      "item": [
        {
          "id": "cba4eb40-ae2e-4fd9-bae2-7b13586cc80a",
          "name": "adminInitiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=AdminInitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56d1ecaa-0871-4ce6-91cd-89e11cf696fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication Challenge",
      "item": [
        {
          "id": "9c297f94-eacf-4430-9761-b371172bdb89",
          "name": "adminRespondToAuthChallenge",
          "request": {
            "url": "http://example.com/api/?Action=AdminRespondToAuthChallenge?ChallengeName=ChallengeName&ChallengeResponses=ChallengeResponses&ClientId=ClientId&Session=Session&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Responds to an authentication challenge, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c913e497-dbd5-40f4-a2fe-db89606ace91"
            }
          ]
        }
      ]
    },
    {
      "name": "Password",
      "item": [
        {
          "id": "0eeeae52-2bef-4fee-bfba-9455decd8cca",
          "name": "changePassword",
          "request": {
            "url": "http://example.com/api/?Action=ChangePassword?AccessToken=AccessToken&PreviousPassword=PreviousPassword&ProposedPassword=ProposedPassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password for a specified user in a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d1af5f0-0cd3-41af-9a2f-717dc09c7a33"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "5f969163-a050-4e94-bd23-1549a30751b9",
          "name": "confirmForgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmForgotPassword?ClientId=ClientId&ConfirmationCode=ConfirmationCode&Password=Password&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to enter a code provided when they reset their password to update\n            their password."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e452bb62-1262-4f01-a755-4025807e9897"
            }
          ]
        },
        {
          "id": "261a4d9d-d7df-4729-85cc-7389fd098429",
          "name": "forgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ForgotPassword?ClientId=ClientId&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the password for the specified client ID or username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6150af42-ad17-47a9-b066-a6e12b782995"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Ups",
      "item": [
        {
          "id": "dc96ebd3-cf2c-4bb1-be23-8090c9a687a3",
          "name": "confirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSignUp?ClientId=ClientId&ConfirmationCode=ConfirmationCode&ForceAliasCreation=ForceAliasCreation&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms registration of a user and handles the existing alias from a previous\n            user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b5551df-1e6d-4c0e-9623-c1ac3a511ec6"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "2595df84-75f5-493d-b930-46c999147fdd",
          "name": "createGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateGroup?Description=Description&GroupName=GroupName&Precedence=Precedence&RoleArn=RoleArn&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new group in the specified user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fd80d05-dbcf-4ad2-a21a-3cfdbce81fdd"
            }
          ]
        },
        {
          "id": "296c1992-804a-44ec-9fbf-fa1549d97e03",
          "name": "deleteGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "654b9de6-d781-40c1-b32a-4b211778a22b"
            }
          ]
        },
        {
          "id": "741c8481-74da-45a5-bb16-311f8d1128d5",
          "name": "getGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f26a9644-4321-4e74-b9bb-0c88f2e1b5f9"
            }
          ]
        },
        {
          "id": "a5289770-4bd9-4117-b196-5d9e434cf210",
          "name": "listGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListGroups?Limit=Limit&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups associated with a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d004164c-e8f4-492f-a840-03b1cb90cf4f"
            }
          ]
        }
      ]
    },
    {
      "name": "CSV Header",
      "item": [
        {
          "id": "0db42f1e-7284-4859-b611-952a54443b50",
          "name": "getCSVHeader",
          "request": {
            "url": "http://example.com/api/?Action=GetCSVHeader?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the header information for the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d83c0a88-4403-4edd-bf82-c7d9d242b018"
            }
          ]
        }
      ]
    },
    {
      "name": "Verification Codes",
      "item": [
        {
          "id": "46216178-bce9-4732-bca0-2f5f9e3e07fb",
          "name": "getUserAttributeVerificationCode",
          "request": {
            "url": "http://example.com/api/?Action=GetUserAttributeVerificationCode?AccessToken=AccessToken&AttributeName=AttributeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attribute verification code for the specified attribute\n            name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d11fadea-82f6-44a2-bc99-987ebebc281d"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Out",
      "item": [
        {
          "id": "060d6a4a-3074-4453-9443-be9c4816e57f",
          "name": "globalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=GlobalSignOut?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3fb6b03-0566-43d9-a2e8-342f96bb976b"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication",
      "item": [
        {
          "id": "c7ba8d83-aa67-4674-b19f-38b4a2f1f5c3",
          "name": "initiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=InitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97c7f6cb-4713-415b-a5c4-d42215ee6562"
            }
          ]
        }
      ]
    }
  ]
}