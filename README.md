# React Todo App Add and Delete

## Adding a todo

Add a todo with the entered title on the form submit:

- text field should be focused by default;
- if the title is empty show the `Title should not be empty` notification at the bottom;
- trim the title when checked or saved;
- use your `userId` for the new todo;
- send a POST request to the API (check the [API Documentation](https://mate-academy.github.io/fe-students-api/))
- disable the input until receiving a response from the API;
- immediately after sending a request create a todo with `id: 0` and save it to the `tempTodo` variable in the state (NOT to the `todos` array);
- show an independent `TodoItem` **after** the list if `tempTodo` is not `null`;
- temp TodoItem should have the loader (check the original markup);
- in case of success add the todo created by the API to the array (take it from the POST response);
- in case of an API error showing `Unable to add a todo` notification at the bottom;
- set `tempTodo` to `null` to hide the extra `TodoItem`;
- focus the text field after receiving a response;
- clear the text in case of success;
- keep the text in case of error;

## Deleting todos

Remove a todo on the `TodoDeleteButton` click:

- covered the todo with the loader while waiting for the API response;
- remove the todo from the list on success;
- in case of API error show `Unable to delete a todo` notification at the bottom (the todo must stay in the list);

Remove all the completed todos after the `Clear completed` button click:

- the button should be enabled only if there is at least 1 completed todo;
- the deletion should work as several individual deletions running at the same time;
- in case of any error show error message but process success deletions;

## Demo Links

- [DEMO LINK](https://AndriiZakharenko.github.io/react_todo-app-add-and-delete/)
