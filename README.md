# spring-boot-akka-cluster-sharding

abc-ms
------
The run1.cmd and run2.cmd starts the abc-ms on HTTP port 7777, 7778 and akka port of 2550 and 2551

def-ms
------
The run3.cmd and run4.cmd starts the def-ms on HTTP port 7779, 7780 and akka port of 2552 and 2553

Sample POST request on abc-ms:
------

http://localhost:7777/abc/event/to/def

Metthod: POST

{
	"eventId": "92242570-5e82-11e5-a2ff-852f495d7e91",
	"eventName": "ACQUIRED",
	"tenantId": "default",
	"createdBy": "test",
	"moduleId": "4b9c21e0-5e7b-11e5-ae4d-852f495d7e91",
	"moduleTypeOfTask": "test type",
	"moduleType": "acquisition",
	"moduleTaskDescription": "aaa desc 233435",
	"assigneeId": "sd",
	"assignedById": "manger",
	"eventType": "ASSIGN"

}


