## What goal will your website be designed to achieve?

This website is meant to give users the ability to browse for information about their local breweries, see the beers they offer. The application will let users keep a log of any visits along with beers they’ve tried. It will serve as a virtual ‘passport’ that makes it easy to keep track of this information.

## What kind of users will visit your site?

Frequenters of breweries and people who love beer are the kinds of users who will visit this site. They will of course need to be legal drinking age. 

## What data do you plan on using?

I plan to use the OpenBrewery  API - https://www.openbrewerydb.org/documentation which contains data about breweries such as their location/address. This api may work better as it includes data about breweries as well as beers ->https://untappd.com/api/docs#breweryinfo 

## Approach Outline

### What does your database schema look like?

The database schema will include tables for users with a username and hashed password. There will be a breweries table that includes the brewery name as well as details about their location. Beers will also need their own table with an association to a brewery, along with details about type of beer and possibly cost. Additionally a table will be needed for visits to track the date a brewery was visited. Finally, an associative table will be needed to match beers with visits. 

https://docs.google.com/spreadsheets/d/1KrYh5jjUowninTFUg8IKIAGtypUjy9k0AFm-cr_k0EA/edit#gid=0 

### What kind of issues might you run into with your API?

The API (or APIs) may be incomplete and/or inaccurate. I may compensate for this by letting users search for breweries or beers but then make their own edits before saving them to the application’s db. On top of that, users can add their own beers. 

### Is there any sensitive information you need to secure?

Passwords will need to be hashed and stored. Otherwise I will minimize use of user info. I may need to require users to confirm their age  before using the app. 

### What functionality will your app include?

The app will provide a function to search for breweries by name or by location. Once one is selected you can log visits and include beers you drank. A user will be able to view a list of breweries they’ve visited (maybe by most recent or most often) and keep track of beers they’ve tried. Users can add their own information about breweries or beers as they need to. 

### What will the user flow look like?

Users will login and see a page listing their favorite breweries (listed by number of visits or most recent visits.) The list will include stats like beers tried and date of last visit. Clicking links into a brewery will show a list of beers tried at that location with info about the dates. Users can search for info about breweries and beers to update.

### What features make your site more than crud?

Having this information stored as a digital passport of the beers you’ve tried at different breweries will let users keep better track of their drinking travels. This will be especially handy for those interested in visiting many breweries and drinking many beers. 

	


