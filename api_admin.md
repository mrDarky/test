##ADMIN RESTful API


###Available requests
| Resource | GET | POST | UPDATE | DALETE |
| --- | --- | --- | --- | --- |
| /projects | return all projects | create new project | - | delete all projects |
GET /projects - return all projects
POST /projects - create new project
DELETE /projects - delete all projects

GET /projects/id - return project with identificator = id
DELETE /projects/id - delete project with identificator = id
UPDATE /project/id - update project with identificator = id


GET /builds - return all current statuses and info about all builds
POST /builds - run all builds in project

GET /builds/id - return current status and info build with identificator = id
POST /builds/id - run build with identificator = id




###Specification
GET /projects - return all projects
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

POST /projects - create new project
* Input format
json
	{
		github_link: link,
		archive: archive_with_sources,
		config_file: file
	}
* Additional arguments for requests
* Output format
Empty response body
* Status codes

DELETE /projects - delete all projects
* Input format
* Additional arguments for requests
* Output format
* Status codes



GET /projects/id - return project with identificator = id
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

DELETE /projects/id - delete project with identificator = id
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

UPDATE /project/id - update project with identificator = id
* Input format
json
	{
		github_link: link,
		archive: archive_with_updates,
		config_file: new_file
	}
* Additional arguments for requests
* Output format
Empty response body
* Status codes



GET /builds - return all current statuses and info about all builds
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

POST /builds - run all builds in project
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

GET /builds/id - return current status and info build with identificator = id
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes

POST /builds/id - run build with identificator = id
* Input format
No input required
* Additional arguments for requests
* Output format
Empty response body
* Status codes