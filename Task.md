# [Week 3]

### Monday:
- Set up a CRUD development environment for the project, including installing necessary software and tools.
- Create a new DynamoDB table to store dealership data, including fields for make, model, year, and price.
- Write code to create a new dealership record in the DynamoDB table using the AWS SDK for JavaScript.

### Tuesday:
- Set up a new React project and create a new component to display dealership data from the DynamoDB table.
- Implement a search feature to allow users to search for dealerships by make, model, year, or price.
- Write code to read dealership records from the DynamoDB table and display them in the React component.

### Wednesday:
- Add functionality to the React component to allow users to edit dealership records.
- Write code to update dealership records in the DynamoDB table using the AWS SDK for JavaScript.
- Test the CRUD functionality of the application to ensure it is working as expected.

### Thursday:
- Integrate Amazon Lex into the application to allow users to interact with the application using natural language.
- Write code to handle user input from Amazon Lex and perform the appropriate CRUD operations in the DynamoDB table.
- Test the application with Amazon Lex to ensure it is working as expected.

### Friday:
- Fixing problems with the e-visa and re-schedule the flights
- Bonding Sections with Freshman Leader Senior from BINUS University

### Saturday:
- Traveling back to hometown for Election

### Sunday:
- Cambodia Election Day

# [Week 4]

### Monday:
- Traveling Back to Workspace
- Orientation Day for Freshman Year Program of BINUS University
	- Zoom (07:30 - 04:00)
- Test the application with Amazon Lex to ensure it is working as expected.
	- Bug Encountered - DynamoDB SDK

### Tuesday:
- Bug fixed: DynamoDB SDK - Reading Items
- Dashboard work perfectly fine with READ and WRITE function
	- Auto refresh at random ms (help avoid too many unnecessary request)
- Bug Encountered Today
	- Lambda: Suddenly stopped writing data to DynamoDB
		- Possible solution: VPC Connection (Doesn't work)
	- Found the error:
		- The error occurred because the lambda function code cannot fulfil the code hook even though the Lex function slots is already filled
		- Possible solution: Make Lambda get Input Value for `event['invocationSource']` to `'FulfillmentCodeHook'` the code will work again and can sent item to database easily.
		- Posted on [stackoverflow](https://stackoverflow.com/questions/76759862/amazon-lex-slots-are-filled-but-lex-responds-to-lambda-said-it-is-still-dialogco)
- Error due to new updates: 
	- Didn't notice the update which break the code
	- Need to read Lambda and Lex new updated documentation

### Wednesday
- Fix any existing bugs in Amazon Lex by reviewing error logs and debugging the code as necessary.
- Read and understand the new version of Amazon Lex, taking note of any changes or new features that may affect the [SearchCar] and [Booking Car Test Drive] functions.
- Rewrite the [Booking Car Test Drive] function to work with the bot and dashboard. This may involve updating the code to use new Lex features or APIs, as well as testing to ensure that the function is working as expected.
- Continue working on rewriting the [SearchCar] function with new Lex updates, taking into account any changes or new features in the latest version. This may involve refactoring the code, updating the API calls, or adding new functionality to improve the user experience.
- Once the bot is finished, integrate the [SearchCar] function with the dashboard. This may involve updating the dashboard UI to display the search results and implementing the necessary API calls to connect the bot and dashboard. Testing should be conducted to ensure that the integration is working as expected.


### Thursday
- Added dialogs to the intents, defining the steps that the bot will take to fulfill a user's intent
- Added Lambda functions to the dialogs, to perform tasks such as retrieving data from a database, making a web request, or generating text
- I need to add more intents and dialogs to the bot to make it more comprehensive
- Test the application with Amazon Lex to ensure it is working as expected
- Switch to working on the front end of car list
	- Card list of available car (model, make, brand, price)
	- Can add car, delete and edit
	- User can retrieve data from the bot

### Friday
- Working on the front-end
- Checking on the back-end
- Attending Lectures

### Saturday


