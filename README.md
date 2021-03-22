![](./Holiday Road Project.png)
# Holiday Road from Nashville
DESC

## Installation
git clone this repository

## Usage
1. `serve` in the project's root directory  
2. `json-server -p 8090 -w db.json` in the project's `"root directory"/api` directory

## Contributing
[Jackson Goodman](https://github.com/jacksonrgoodman)  
[Colten Mayberry](https://github.com/coltmay)  
[Sidney Crandall](https://github.com/SidneyCrandall)  
[Bre Coach](https://github.com/Coachbre)  

## License
[MIT](https://choosealicense.com/licenses/mit/)

# PROJECT OUTLINE AND GOALS
You and your teammates have been contracted by the National Parks Service to build an application that will allow people to build itineraries for their trips to the beautiful national parks that they maintain. The starting point of each trip will be Nashville, TN, but the destination will a national park selected by the user.

## Getting Started

This is going to be your first full, professional Sprint. A Sprint is part of the [Scrum Framework](https://en.wikipedia.org/wiki/Scrum_%28software_development%29) for agile development. You will be doing daily scrum stand-ups, where you provide a concise status update on your own work. You will be taking part in a sprint review where you demonstrate the work you have completed. You will be taking part in a retrospective, where the team reflects on the work done, the team dynamics, and discuss how to improve in the future.

### Code Review

During this sprint, the focus will be on learning, much more than doing. We estimate that most teams could get this project done in 2-3 days. We are giving you 5.

To accomplish maximum learning, the following requirement is placed on the team, and will be monitored by your team lead. When a teammate submits a PR, and you are ready to review it, then you and the submitter must sit together and review all of the code that was written. Also, if any other teammates would like to review the code, then you must include them on the review.

Only when you feel you understand all of the code, you may then complete testing of the feature and provide approval for merging.

### Settings

After each teammate clone the repository, each must perform the following steps.

1. In the `scripts` directory, you will see a file named `Settings.js.example`.
1. Copy that file with `cp Settings.js.example Settings.js`. The `Settings.js` file is already in the `.gitignore` file, so it won't ever be tracked by git.
1. Make a copy of the `db.json.example` file in the `api` directory without the `.example` extension: `cp db.json.example db.json`. The `db.json` file is already in the `.gitignore` file, so it won't ever be tracked by git.
1. Register an API key for the APIs below that need it.
1. Copy your key into the appropriate place in the `Settings.js` file.
1. The team will need to figure out how to import that object into the data provider modules and use it for the `fetch()` calls that need to be performed.

**_DO NOT MODIFY Settings.js.example OR db.json.example during this project!!!_**

## Feature List

### Building the Itinerary

* List all national parks in a dropdown. When user chooses one, display the name of the park in the **Itinerary Preview** section.

* List all bizarraries in a dropdown. When user chooses one, display the name of the bizarre attraction in the **Itinerary Preview** section.

* List all eateries in a dropdown. When user chooses one, display the name of the eatery in the **Itinerary Preview** section.

### Itinerary Details

* In the **Itinerary Preview** section, there should be a button labeled _Save Itinerary_. It should be disabled by default.
* When the user has selected a park, and the name of the park has been added to the **Itinerary Preview** section, query the Open Weather API and display the 5 day forecast for that location. This will allow the user to see if they want to make the trip soon.
* When the user adds any item to the **Itinerary Preview**, there should be a _Details_ button next to the name of the item.

* When the user clicks on any detail button for an itinerary item, a dialog box should be presented to the user with more information about that item _(description, address, etc...)_.
* Once the user has selected a park, a bizarre attraction, and an eatery, the _Save Itinerary_ button should be enabled.
* When the user clicks the _Save Itinerary_ button, the chosen items should be saved as an object in your own, local API that is managed by `json-server`. Each saved itinerary should appear in an aside bar on the right side of the UI.


### Brittany

![](./personas/persona-brittany.png)
