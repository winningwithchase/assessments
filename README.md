# Assessment - Interviews UI

## Prompt

You are tasked with building a UI that can create interviews and display a list of interviews associated with an account.

This UI must interact with our `example-api` with details provided below.

The API is provided at `http://example-api.winningwithchase.com` and [the API documentation details the two routes available](http://example-api.winningwithchase.com/docs).

## Deliverable

- Compressed folder containing your code; i.e., `.zip` file

This folder should contain a README with instructions on how to run it.

Please do not include `/node_modules`. Put all your packages in `package.json` and we will install them ourselves.

Any supplemental documentation on your design and process are welcome!

## Making requests against the API

### Documentation

[Interactive API Docs. Use these to test your requests out before writing code if you want.](http://example-api.winningwithchase.com/docs)

### Authentication

Instead of authentication we have a very simple mechanism for managing accounts.

Simply pass the `account-id` as a header with a [Universally Unique Identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier).

You are responsible for generating this ID and persisting it in the state of your UI.

### Passing scheduled_at

The `scheduled_at` param in the object is an [ISO-8601 datetime string](https://en.wikipedia.org/wiki/ISO_8601).

## Extra-Credit

To showcase your strengths there are extra-credit in both frontend and backend capacities.

If your backend skills are stronger than your frontend feel free to focus more on building the application end-to-end.

### Frontend

- Style the interview cards and list view
- Put Create Interview form in a Modal
- Clean UI for picking scheduled_at time (better than a textbox)

### Backend

- Build the two routes GET/POST /interview (no DB necessary, in memory is fine)
- Add a DELETE route for deleting interviews by `interview_id` (bonus if you add the DELETE button to the frontend)
