# Car-dekho-challenge

## Requirement
MongoDB for database
React for front-end

## Server-side
- We've provided some .csv files, use them to store some details into MongoDB.
- Make a route `/user/login` for user login.
- Make a route `/user/register`for user resigtation.
- Make a route `/car/details` for fetching the details for the car based of selected make, model, and trim.
  - It should have some query params:

  - For eg I'd like to fetch a list of make:
    - `/car/details?cmd='getMakes'`
  - For eg I'd like to fetch model for make='audi':
    - `/car/details?cmd='getModels'&make="audi"`
  - For eg I'd like to fetch trims for make='audi' and model='A3':
    - `/car/details?cmd='getTrims'&make="audi"&model="A3"`
  - Show all the details of trims in the page which is defined in trim.csv file.

## Client-side
We need a site where we want to show car details based on some filters.
- Make a login page, ask for username and password.
- Redirect to `/cars` page after login.
  - This page should have some dropdowns to show all the details of the filtered cars, and a button `Show Data`.
    - make
    - model
    - trim
  - By defaut the page will show only the dropdowns(mentioned above), and only make dropdown will be populated.
  - After selecting 1 item from the make dropdown, then the model dropdown should get populated (list will come from an api call).
  - After selecting 1 item from the model dropdown, then the trim dropdown should get populated (list will come from an api call).
  - and so on.
  - At last clicking on the button, should show the details(defined in the trim.csv file).
  - There should also contain a toggle to show the list into grid view or list view.
- There should be a button to navigate it to `/admin` route. From admin page only admin user could add new car details,
  it should be done in way that when we add a new car details first check the user authentication for admin/non-admin user. (Use JWT token for auth)
- When admin user is adding a new car details, then it should be real-time(Preferably GraphQL, socket.io). To do that, add a new
  detail in 1 browser and check in another browser that without reloading the page, can we see the newly added car details or not.
  
  
## Deliverables
 - Checkout a branch of your name from the master branch.
 - Complete this challenge in that branch with proper commits.
 - Code should be very clean and understandable.
 - Project should be run error free.
 - Make a file where you tell us about the challenges you came across and how you solved it.
 - How much time taken to complete this challenge, shorter time is the best.
