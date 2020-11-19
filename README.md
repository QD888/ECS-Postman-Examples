# ECS Postman Examples

This repository hold templated Postman collections for common API commands for

[Dell Technologies Elastic Cloud Storage]: https://www.delltechnologies.com/en-au/storage/ecs/index.htm

(ECS) product.

There are two collections which span Management and S3 API usage.  These collections have been tested and used against 

[]: https://portal.ecstestdrive.com/	"ECS Test Drive ECS Test Drive and an ECS 3.5 cluster."

When you import these collections into your Postman instance you will also need to import the Postman Environment Variables.  You will then need to fill out the current values for most of the variables to have the collections working in the way they have been designed.

Below is a table explaining that each variable field is and what type of values are needed.

| Variables    | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| endpoint     | Add your ECS S3 data endpoint address.  If you are going direct to an ECS node you might need to add the S3 port number to the end of the endpoint.<br />Example https://object.ecstestdrive.com{PORT_NUM} |
| endpointmtg  | Add the ECS management endpoint with the management port number 4443. Exmaple https://portal.ecstestdrive.com:4443 |
| accessKey    | ECS S3 object user. *Note this is ECS classic user authentication which works on all ECS software versions.* |
| secretKey    | ECS S3 object user secret. Note this is ECS classic user authentication which works on all ECS software versions. |
| username     | ECS Management User                                          |
| password     | ECS Management password                                      |
| namespace    | **Optional,** this is an ECS namespace if you want to limit some commands to a specific namespace. |
| bucket       | **Optional**, if you want to limit some commands to a specific bucket. |
| iamAccessKey | ECS IAM User. *Note requires ECS minimum 3.5*                |
| iamSecret    | ECS IAM User secret.  *Note requires ECS minimum 3.5*        |
| token        | The token field is used in the postman code to store the management token after you login. |

