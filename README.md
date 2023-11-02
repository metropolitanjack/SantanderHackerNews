# SantanderHackerNews

Running StoryBlast api in the HackerBlast project

Method 1: Open the project in Visual Studio 2022, Run the project, test in swagger

Method 2: 

	Build the project in Visual Studio 2022, 
 
	In a command line console navigate to <projectroot>\HackerBlast\HackerBlast\bin\Debug\net6.0
 
	run cmd HackerBlast.exe
 
	Open a browser to https://localhost:5001/api/StoryBlast?n=9   (to show 9 results).

Assumptions

	(1) The list of story id's returned by https://hacker-news.firebaseio.com/v0/beststories.json is in descending order of score
 	
  	(2) Changing attributes of the story (comment count etc) mean that its better to get the details each time 
		(otherwise we could also cache the details and retrieve from a threadsafe dictionary)

Running the Tests:
	In Visual Studio, Test Menu -> Run all tests.
