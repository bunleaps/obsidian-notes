# Contact Flows
### Basic Contact Flows
Timeout - if user doesn't choose any choices and exceed the timeout
Default - if user choose something other than the choices provided
Error - encounter error

DTMF - pressing pad number on phone
	Can put Options

Amazon Lex - chat system for IVR using advanced language

Set working queue - Select specific queue to transfer to
Transfer to queue - transfer to the exact queue picked in set working queue

We can also check with Check Block (ex. Hours of Operation)

Play prompt - TTS 

Default - Sorry, this is an invalid options
Error - Sorry an error occurred. This call is being disconnected. Please call back later.

Transfer --> At capacity: Sorry all our agents are busy at the moment, please call back later

### 9 Types of Contact Flows
Need to choose appropriate type of flows
1. Contact Flows (Generic Contact Flow)
2. Customer Queue Flow
3. Customer Hold Flow
4. Customer Whisper Flow
5. Outbound Whisper Flow
6. Agent Hold Flow
7. Agent Whisper Flow
8. Transfer to Agent Flow
9. Transfer to Queue Flow

For Phone Number can only be used with Generic Contact Flow

Each of those types have unique purpose and different building block flow

Customer Queue Flow is what customer experience after transfer to the queue

Mermaid Graph
Get Customer Input --> Set Working Queue --> Transfer to Queue --> Customer Queue Flow

Loop prompts
Loop through events list
1. TTS
2. Music
3. Commercial

It is not recommended to use or change default flow, always create a new one

### Contact Attributes
Contact Attributes are key-value pairs that contain fata about a contact (phone call or chat)

KEY      -       VALUE Pairs
Customer Phone Number: +64 12 345 6789
Contact Channel: Chat
Queue Name: Sales

Types of Contact Attributes
1. System (Pre define, queue name)
2. Agent (agent first name, last name)
3. Queue Metrics (Number of customer, agent available)
4. Customer (customer first name, last name, profile)
5. Media Streams (timestamps)
6. Lex Slots (Amazon Lex)
7. Lex Attributes (Amazon Lex)
8. External (Lambda)
9. User-defined (Created during contact flow, variable)

Attribute list
docs.aws.amazon.com/connect/latest/adminguide/connect-attrib-list.html

Polly SSML - Speech Synthesis Markup Language
