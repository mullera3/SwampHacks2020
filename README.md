# SwampHacks2020

Inspiration
We are all college students and have all run into the problem of having limited storage. Most storage units are way too big for the number of belongings we have (which take up valuable environmental space as well as upkeep costs) and are in turn way too expensive. We set out to find a solution to this.

What it does
In our app, the user can say what exactly they need to be stored (with characteristics such as size, brands, etc.). They would also be able to specify if they want to pay an extra fee to have it picked up by one of our delivery drivers, or if they would like to drop it off at our fulfillment center themselves. We also send out reminders through text to update users on their pickup status. Their belongings are then tracked with our barcode system and stored in just the right amount of space to keep costs low for the user. Once they would like to retrieve their items from storage, they simply go in the app and can pay an additional fee if they would like it delivered. Just like text notifications are given to pickup status, the same idea was implemented for retrieval status.

How we built it
With great difficulty...but for real, the bulk of the code was written in Python and is backboned by an SQL database. All of the queries for the database were driven using Python as well. In addition to this, we offered some other features, such as text notifications and barcode creation. The text notifications were handled by the Twilio SMS API paired with authentification ID and token which are tied to the user's S'MORE account. The barcodes were created using special Python class implementations.

Challenges we ran into
Running SQL through Python was quite an undertaking. None of us had really worked with the combination before and it took some R&D to get things working. Another challenge was the barcodes. We initially started trying to implement QR codes, but after struggling and understanding that they were more advantageous in web applications, we shifted our focus to procedurally generated barcodes backed by EAN13.

Accomplishments that we're proud of
None of us really had a lot of experience dealing with APIs, so being able to properly use the Twilio API was a very proud moment for us. In addition to this, we are very proud of our UI design and how clean the interface is to work with.

What we learned
No pain, no gain. Things seemed bleak during the middle of the hackathon, but we pushed through and made it in the end.

What's next for S'MORE
We would like to focus on solidifying our financial agreements with users, and possibly look into using NCR's catalog API to handle pricing. In addition to this, we would like to use Kivy to create a better link with our frontend and backend
