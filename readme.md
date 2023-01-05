#### Making the URL

- This is the url given to us ` var queryURL = "https://api.nytimes.com/svc/search/v2/articlesearch.json?";`
- Our form has 4 fields, and while sending the request to New york's api our url should include values from those input fields.


It becomes like this after adding the input field values
- `https://api.nytimes.com/svc/search/v2/articlesearch.json?api-key=R1a31F4tBjCUaM2ho8GtIFsrSdtXt30M&q=ronaldo&begin_date=20110101&end_date=20220101`
- After the `?` there is `api-key=value`, then we have `q=value` which will hold the value of search term.
- Then we have `begin_date=20110101`, the value `20110101` means the value added to input field was `2011` but while sending that value to the url, you need to add `0101` to its end so it becomes `20110101`. (This is how new york's api is expecting us to send data this is not any general rule!!)
- Same instructions for `end_date` in the URL