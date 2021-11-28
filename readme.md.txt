Feature 2:
As a user, I should be able to show/hide an event’s details, so that I can limit the amount of information someone can view.
Scenario 1: An event element is collapsed by default
Given a user is viewing events on the main view
When events are being displayed
Then the event details are collapsed
Scenario 2: User can expand an event to see it’s details
Given a user is looking at an events on the main view
When that event is selected and the show details button is clicked
Then the event’s details are displayed
Scenario 3: Users can collapse an event to hide it’s details
Given a user is looking at events on the main view
When that event is selected and the hide details button is clicked
Then the event’s details are collapsed and hidden

Feature 3:
As a user, I should be able to specify the number of events shown, so that I can browse the information at my own pace
Scenario 1: When the user hasn’t specified a number 32 is the default number
Given the user is currently searching for events
When the user enters their search without specifying how many events to be shown
Then the default number of events shown would be 32
Scenario 2: User can change the number of events they want to see
Given the user is searching for events
When the user specifies how many events they want to see on a search
Then the user’s specified number for events will show that many events
Feature 4:
As a user, I should be able to use the app offline, so that I can remind myself of events even when not connected to the internet
Scenario 1: Show cached data when there is no internet connection
Given the user is offline
When the user is trying to access the application
Then the cached data for the user will be shown
Scenario 2: Show error message when user changes settings (city, time, range)
Given the user is offline
When the user is trying to change their settings
Then the application will display an error message
Feature 5:
As a user, I should be able to visualize the data of my events, so that I can have an easier time keeping track of them.
Scenario 1: Shows a chart with the number of upcoming events in each city
Given the user is searching for events
When the user chooses the option to have a chart displaying events
Then the upcoming events in each city will be displayed in a chart