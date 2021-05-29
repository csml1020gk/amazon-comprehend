# amazon-comprehend
Find insights and relationships in text 
https://aws.amazon.com/blogs/machine-learning/deriving-conversational-insights-from-invoices-with-amazon-textract-amazon-comprehend-and-amazon-lex/

Do you have physical documents to process ?
Does your work involve extraction of information from scanned documents?
You might be using OCR, manual effort or custm code.

Automate text data processing and insight discovery 


Extract text from receipts or invoices in pdf or images with Amazon Textract.
Derive insights with Amazon Comprehend.
Interact with these insights in natural language using Amazon Lex.

Backend user/admin uploads raw data to S3 bucket 
Amazon S3 bucket triggers lambda function to invocke Textract to extract text from the document 
When text processing is complete, Textract triggers a SNS message which invokes another at to detect the text and load to s3 bucket
Another lambda function is used to detect intents using Comprehend which performs entity and key phrases detection 
User types a message - bot detects the intent type and invokes appropriate API 
Deploy the Lexot WeUI 

Confirm this project can be completed on Free Tier account 

Services used           : Availability on free tier 

cognito                 : 
lambda                  :
lex                     :
comprehend              :
textract                :
s3                      :



