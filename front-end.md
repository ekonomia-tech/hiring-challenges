# Frontend Challange

This test will assess your ability to connect to a data storing mechanism, query it, and present the results in a simple react project.

## Stack
- React\Preact\Svelete\SolidJS - your choice.
- GraphQL querying library - you can decide which one you want to use.
- Any other library that will help you reach the goal is acceptable. But try to limit the amount of libraries you are using as much as possible.
- Try to reduce the bundle size as much as possible (you can use Preact if you want).

## Objectives
- Connect to a GraphQL subgraph on the following api: https://api.thegraph.com/subgraphs/name/nmimran99/defi-subgraphs
- Create 2 pages
  - Accounts page - a page with a table that presents accounts (description below)
  - Account description - a page that has different data elements in a context of a single account (description below)
- Create the routing between the pages

#### Accounts page
- Create a page that will present 10 different accounts on every page from the subgraph mentioned above
- Create a table that will have the following columns
  - `accountID` - a link to an account description page
    - `onClick` - route to the account description page
  - Number of positions the account has (count)
- Make sure the table has pagination capabilities. moving to the next page should present the next 10 accounts.
- Limit the number of total accounts to 100.

#### Account description page
Create a page that will aggregate the account's activities
The page should consist of:
- A header with the `accountID`
- A list of protocols the account have interacted with Protocol Icon and Name. Can be aggregated from `events` entity
- A table that shows the following:
  - Market ID
  - Asset Name
  - Amount of decimals for the asset
  - Total deposited
  - Total withdrawn
  - Total borrowed
  - Total repaid

## Submission
You can work on a private GitHub repo and then share it with **davekaj** GitHub user. Feel free to send any question while doing the exercise.
