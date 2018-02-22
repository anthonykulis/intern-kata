# Intern Kata

The goal of this kata is to show you understand the React/Redux flow, as well as React routing flow at a junior developer level. You will query a set of APIs using all CRUD operations as well as Search.

## Directions

Extending out what we did on the catfish kata, you will now build a form for administrators of the catfish tournament to maintain records.

* You will create a simple form to submit a new entry (Create operation)
* You will create a table to view the entries (Read operation), sortable by name, species, weight, or date caught that allows the tournament administrator to perform the Update and Delete operations.
* When the administrator wishes to update an entry, the previously mentioned form fields will be populated and the submission handled there.
* Lastly, to perform the search portion, there should be a form field that searches the entries by what the administrator has typed in. This could be any of the data columns. While typically we'd do this search on the server, we have no choice but to do it locally.

### Limitations
Since this is hitting mock servers, there are some limitations.
* You do not need to paginate the results. There are 100 records and you can read them all at once
* When you do any CRUD operation that has server side effects, you should maintain those side effects locally. This means any POST, PUT, or DELETE operations should hit the mock server, but for kata reasons, the reducer should respond as if the server just sent back a 200 and never any data. Hint, you will need to update your actions slightly to pass the data to the reducer as something besides payload so you can maintain state.

### Tools
You are allowed to use any tools, including `@chassi-dev/chassi-react-mui-components` or any other npm we host.

## UI
UI isnt as important as logic here. I include a simple UI in the repo you can reference. The only thing I ask is that you use table headers of `Angler Name - Species - Weight - Date - Manage` and the rows have the corresponding values and manage has an edit and delete icon. The MUI components table in the storybook has great examples.

## Expectations
You are expected to properly build out the React/Redux flow, meaning the proper logic is in the proper parts of the flow (action -> reducer -> store -> ui). Remember, inside the UI putting code in proper places matter as well. Use the redux tools effectively and properly.

You are also expected to write code. Avoid copy and pasting. I will be looking for copy paste in my evaluation. You may however use any existing code as reference material.

Finally, you are expected to commit each day until the project is finished. Make sure you commits are logical and granular. Make sure I am tagged some how. Feel free to do PRs on your fork of this and make me a reviewer for the PR. You do not need to tag me on each commit when you do this because github will notify me of the PR when you put me on as a review.

## Evaluation
You will be evaluated on the proper logic of code residing in the proper spots of the React/Redux flow and in the proper spots of the React component lifecyle.

## Seeking help
You are encouraged to seek help and guidance. Somethings are expected, meaning you are expected to be able to solve them on your own (see expectations). If a question is too much related to the expectations, I will direct you to the react and/or redux documentation.
