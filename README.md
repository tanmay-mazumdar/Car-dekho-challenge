# Car-dekho-challenge

## Requirement
MongoDB for database
React for front-end

## Server-side
- Make a route `/user/login` for user login.
- Make a route `/user/register`for user resigtation.
- Make a route that could send the list of model of a selected make or trims of a selected model.
- Make a route `/car/details` for fetching the details for the car based of selected make, model, and trim.
  - It should have some query params:
    - make='all' -> Get a list of all the makes. 'all' means all, otherwise provide a specific make.
    - model='all' -> Get a list of all the models.'all' means all, otherwise provide a specific model.
    - trim='all' -> Get a list of all the trim. 'all' means all, otherwise provide a specific trim.
  - For eg I'd like to fetch details for make='audi', model='A3', trim='1.9 TDI AT' then the route will be.
    - `/car/details?make="audi"&model="A3"&trim="1.9 TDI AT"`
  - Make methods to enter of all the data from the csv file we have provided in this repo.

## Client-side
We need a site where we want to show car details based on some filters.
- Make a login page, ask for username and password.
- Redirect to `/cars` page after login.
  - This page should have some dropdowns to show all the details of the filtered cars.
    - make
    - model
    - generation
    - series
    - trim
    - equipment
  - By defaut the page will show only the dropdowns(mentioned above), and only make dropdown will be populated.
  - After selecting 1 item from the make dropdown, then the model dropdown should get populated (list will come from an api call).
  - After selecting 1 item from the model dropdown, then the generating dropdown should get populated (list will come from an api call).
  - and so on.
  - At last there should be a button to show the filtered data in the form of list.
  - There should also contain a toggle to show the list into grid view or list view.
  
  
## Deliverables
 - Checkout a branch of your name from the master branch.
 - Complete this challenge in that branch with proper commits.
 - Code should be very clean and understandable.
 - Project should be run error free.
 - Make a file where you tell us about the challenges you came across and how you solved it.
 - How much time taken to complete this challenge, shorter time is the best.
