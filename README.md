# instagram-scraper

####Python script to scrape Instagram public accounts data using official API & store in a MySQL Database.

#####Below are the high level workflow features of the program.

 
- Fetch 'x' number of Instgaram users IDs from source, a MySQL Database table hosted on AWS Cloud.
- Fetch list Followers & their metadat details on Instagram for each accounts in parallel.
- Store the result of Followers list for each account in an Output table in MySQL Database.
- Repeat the process indefinetly.
- If all accounts data fetched, wait/sleep until new list of accounts is added to the table.
- Automatically Retry if any request to Instagram API fails.
- Use random session cookie ids for each requests to avoid account blocking by Instagram.
- Use proxy server to rotate IPs.
- The program can be run as Docker container and deployed to any cloud or on-premise Infrastructure.
