# Crowdfunding Back End
{{ your name here }}

## Planning:
### Concept/Name
{{ Include a short description of your website concept here. }}

### Intended Audience/User Stories
{{ Who are your intended audience? How will they use the website? }}

### Front End Pages/Functionality
-Home Page
    - Featured fundraiser
- Search Page
  - search specific fundraiser
- Create new fundraiser page
  - form with fundraiser details
  - abilty to submit
  - nice error pages for validation
- Display Fundraiser
  - shows all information about fundraiser
  - show all pledges made so far
  
### API Spec
{{ Fill out the table below to define your endpoints. An example of what this might look like is shown at the bottom of the page. 

It might look messy here in the PDF, but once it's rendered it looks very neat! 

It can be helpful to keep the markdown preview open in VS Code so that you can see what you're typing more easily. }}

| URL           | HTTP Method | Purpose                   | Request Body | Success Response Code | Authentication/Authorisation             |
| ------------- | ----------- | ------------------------- | ------------ | --------------------- | ---------------------------------------- |
| /fundraisers/ | GET         | Fetch all the fundrasiers | N/A          | 200                   | None                                     |
| /fundraisers/ | POST        | Create a new fundraiser   | JSON Payload | 201                   | Any logged in user                       |
| /fundraisers/ | PUT         | Update fundraiser         | JSON Payload | 200                   | Logged in fundraiser owner               |
| /pledges/     | GET         | Fetch all the pledges     | N/A          | 200                   | Users who've pledged to the same project |
| /pledges/     | POST        | Creating a new pledge     | JSON Payload | 201                   | Logged in user                           |
| /pledges/     | PUT         | Update pledges            | JSON Payload | 200                   | Logged in pledge owner                   |
| /users/       | GET         | Fetch all users           | N/A          | 200                   | None                                     | Admin |
| /users        | POST        | Create new user           | JSON Payload | 201                   | None                                     |
| /users/       | PUT         | Update user               | JSON Payload | 200                   | Logged in user                           |

### DB Schema
![](./database.drawio.svg)