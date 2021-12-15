# DealerMine Junior Full Stack Coding Challenge

## Setup
- Make a private clone of the repo and do all of your work inside of this clone
  - Click 'use this template' on the top right of the GitHub page and create a private clone
  - IMPORTANT: Do not fork this repository, as the fork will be publicly-visible (consider using a new GitHub account if you are concerned about discretion)
- Complete the code to solve the problem described below
- Create a small technical write-up that describes how you solved the problem, and put it in DESCRIPTION.md
- Add **@ccrane-quorum** to the private repository and send an e-mail to chris.crane@quoruminfotech.com once you've pushed your completed project up to GitHub

## Challenge Details
### Implement a search result list for hotels
 - Use a .NET tech stack and C#.
 - When the user clicks the ***Load Hotels*** button, the data for the hotels should be received from the API endpoint with an AJAX call.
 - If the request was successful, show a list of hotels and associated data. 
 - If not, show an appropriate error message
 - When the user clicks on a ***Show Reviews*** button, the reviews should be loaded for this specific hotel.
 - Show the reviews in a list below the hotel information, but inside the hotel item container.
 - Your results page should use web design best practices.
 - Each call to the Fake Hotel API should be logged in a database.
    - Provide a sql script to create the database and table structure.
    - Each log entry should include which endpoint was called (hotels or reviews), when it was called, and the count to items returned if successfull, and error message if unsuccessful
 - Use xUnit v2 to create any necessary Unit tests.

### API endpoint
The required hotel data is available via the Fake Hotel API. All needed documentation is published on http://fake-hotel-api.herokuapp.com/

### Additional requirements
Should run without errors on current versions of Firefox, Chrome and Safari, and Microsoft Edge. HTML should be valid for current HTML5 standards. Responsive behavior is not requested, but feel free to be creative!

### Fake Hotel API Sample Reponses
#### http://fake-hotel-api.herokuapp.com/api/hotels
```[
  {
    "id": "13ef1108-7f18-40c7-ac0f-0e743b015755", //hotel id
    "name": "soluta aperiam rerum", //hotel name
    "country": "Seychelles", //hotel country
    "city": "Norbertberg", //hotel city
    "price": 140, //offer price
    "images": [ //hotel images
      "http://lorempixel.com/640/480/city?87325",
      ...
    ],
    "date_start": "2016-04-02T08:09:12.088Z", //offer start date
    "date_end": "2016-11-30T04:27:59.359Z", //offer end date
    "stars": 2, //hotel stars
    "rating": 1.811553610023111, //hotel rating
    "description": "Recusandae enim debitis quisquam pariatur..." //hotel description
  },
  ...
]
```
#### http://fake-hotel-api.herokuapp.com/api/reviews
```
[
  {
    "name": "Nigel Kub", //commenter name
    "comment": "Rerum est suscipit adipisci odio hic.", //comment
    "positive": true, //false if comment is negative
    "hotel_id": "13ef1108-7f18-40c7-ac0f-0e743b015755" //hotel id
  },
  ...
]
```
#### Error Response
```
{
  "error": "Something failed!" //error message
}
```

## Final Comments
If you require additional details or clarification on any part of this code challenge please send an email to chris.crane@quoruminfotech.com with the subject line ***DealerMine Junior Full Stack Code Challenge - Inquiry***.

**Good luck** :smiley:
