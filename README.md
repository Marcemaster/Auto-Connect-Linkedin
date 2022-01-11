# Auto-Connect-Linkedin
JS script to send connection requests to your LinkedIn search results with customisation option


### What is this?
So, have you ever wanted to connect to people on LinkedIn who are recruiters at X company or study at Y university or work at Z and more. What we usually do is search for "recruiter X", then choose People and start sending connect request to them. This is a manual task, and the conversion rate is very low; so after sending 100 requests to people, 10 accept your request in the best case. What can you do to increase your chances and acceptance? Obviously, you won't sit and send it to 1000 people, right? That's where the script comes in.

The script, once run (instructions below), works in the background on the page and keeps on sending connection requests to the results on the page as long as either it meets maximum requests specified by you or there are no more results. This allows you to just search, run the script, keep the tab open and forget about it. The script has an adequate amount of delay placed between actions so you are not banned, and your connections to the particular company have higher chances of increasing 😄

How to use the above script?
Open Linkedin, search for terms such as "Amazon recruiter", choose People, choose 2nd and 3rd+ connection level.
Open the developer console of your browser following the instructions here for your browser.
Copy the entire above script and paste it into the console and hit enter.
Do not close or refresh the browser tab unless you want the script to stop abruptly.
You'll see that connection requests are being sent now after delays set in the config of the above file. If you want to limit the number of connections to be sent, please update maxRequests above to the desired number of requests.

### When does the script stop?
When there is no next button.
When there are no search results on the current page.
When the number of max requests (if specified) is reached.
What to configure?
If it is taking too long or you are on a very fast internet connection, you can lower the delays between each action since elements will be loading faster for you. Below is an explanation of what each of the configuration item does:

scrollDelay: specifies the wait in milliseconds after scrolling page to bottom and top to load results fully into the page.
actionDelay: specifies the delay in milliseconds between each action such as pressing the connect button, then the done button, and so on.
nextPageDelay: specifies the wait in milliseconds for the next page to load after pressing the next page button.
maxRequests: set to a positive number to limit the number of connection requests to be sent to that number; a negative number leads to infinite connection requests (not really).
totalRequestsSent: stores the number of total requests sent (displayed when the script stops gracefully) and is not to be changed, and should remain 0.
addNote: set to true if you wish to add a note in your invites, otherwise `false.
note: the text of the note to be sent; if it is an empty string, no note is added. You can also add the first name of the person by using the placeholder "{{name}}" (without quotes, with curly brackets).
Acknowledgement
