<H1> Welcome to the YouTube NewsLetteter </H1>

The purpose of this function is to be able to create a list of youtube subscribers that might want to be a part of your channel's emailing list! These
are very basic functions however it could be useful depending on how you might want to apply it's use. 

There are two distinct functions that you will be able to use.
- the first one is {URL}/create POST (Here the user will input their email)
	The expected input is the subscribers email in plain text and the return will be (Status 200 OK) the body will also return an "OK"
	
- the second one is {URL}/findAll GET (Here you will be able to get a list of your subscriber's email)
	For this functions you will not need an input as there will only be a return. Here the return should also be a (Status 200 OK) as
	well as the list of emails 

These were create with spring cloud so if you are going to test these out first you will need to make a couple additions to your header on postman.
For your header you will need to add the following key - spring.cloud.function.definition
The value is interchangable. if you are registering an email the value will be "create"
if you are trying to get a list of the subscribers the value will "findAll"

These lambda functions were stored on aws cloud and it is currently up and running. if needed the url will be disclosed upon request.
