Steps to run:

Run the Server to enable mocking HTTP Req
	1. In the folder MockServer, open it in any editor preferably VSC and give the command npx json-server --watch src/db.json
	2. This will start the mock server  (URL: http://localhost:3000)

Run the Frontend
	1. Open the folder FraunhoferTask in Visual Studio preferably and in the terminal give the commands
		npm install //to install the dependencies and then
		npm start.
	2. It will to run on the port 3001 ( URL: http://localhost:3001)
	

Some Notes:
		1. I was facing errors in the second user story so I implemented only the line Plot. But that also 
		is not working. Looks to me of d3.line issue. I didnt have enough time or else I would have 
		debugged it.
		2. In the first user story, for the hovering part, I tried to add tooltip to show the id of 
			the hovered point. But it didnt work. Looks to me the event issue of fetching the
			mouse coordinates. So simply shown the id without any toolTip, due to time contstraints.

Ambiguity: I found that, there are points where the id is same for multiple points, this creates 
			a problem when trying to fetch the corresponding curve, since the id is the only uniqueness,
			and therefore, the righly mapped curve may not be retreived due to multiple same IDs.
		
		 
