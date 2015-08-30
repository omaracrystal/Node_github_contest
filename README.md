# Node Github Contest App

Let's create an Express app that simulates a contest - adding submissions, voting on a submission, determining a winner!

## Part 1 - setup

1. Create an Express boilerplate using the Express Generator.
1. Add all logic/code to the *routes/index.js* folder.
1. Create a `Submission` class that has the following attributes - `githubName`, `githubURL`, `githubImage`.

## Part 2 - submissions

1. Create a page where the end user can submit an entry.
1. Add a route to handle the form submission. On submit, this should create a new `Submission` instance, adding it to an array.
1. Add logic to stop adding submissions after 8 submissions. Display an error message when a user attempts to add a submission after 8 submissions.

## Part 3 - voting

1. Create a page to display submissions in competing pairs.
1. Allow the user to vote as many times as they want. After a vote, make sure to send a POST request to the server to increment the vote for that specific submission.

## Part 4 - winner

1. Add a button to the bottom of the submission page to determine a winner for the current round. There should be three rounds (8 submissions, 4 submissions, 2 submissions).
1. When a round is complete, the submissions page should update, again, displaying submissions in competing pairs.
1. When a winner is crowned, add a new button to allow the contest to start over! Once pressed, redirect the user to the submissions page to add new submissions.
