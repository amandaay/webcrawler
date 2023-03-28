# Webcrawler Project

## CS5700 Computer Networking

### Briefly describe your high-level approach (all steps involved in logging in, crawling and getting the secret Flags)
We have first created a class according to [html parser library](https://docs.python.org/3/library/html.parser.html). We captured all the tags that will include ‘a’ tag for the urls to be crawled and make sure it will not be revisited. We also include the ‘input’ tag to search for the middleware token. Finally, we used the “handle_data” function to search for the secret flag.
### Any challenges you faced
- One of the major challenges we faced was to handle the receive function, which involves a lot of byte and string conversion and parsing.
- Parsed receiving data.
- Adjusted the handle_starttag methods in the FakebookHTMLParser so that it can get the special tag properly.
### An overview of how you tested your code
- We mainly started off by simply printing line-by-line when we had issues and debug starting at that point where we found issues.
- We then replaced the empty string in our username and password in the parse_cmd_line() function
- We commented out sys.argv[1] and sys.argv[2], so we can test in console first.
### You must also include a breakdown of who worked on what part(s) of the code. Also, give us the steps on how to run your code.
- Each of us started our own research and finished 80% of the code. Then we met at a zoom meeting to discuss errors and issues we encountered. And finalized the project with the remaining 20%.
- [Amanda](https://github.com/amandaay) @amandaay: mainly focused on writing the html parser class, receiver function
- [Wayne](https://github.com/Chun-Wei-Tseng) @Chun-Wei-Tseng: mainly focused on get request function, cookie jar
- [Jason](https://github.com/JasonKTChen) @JasonKTChen: mainly focused on login_user, start_crawling and main


## Team's Terminal URL execution
- [Amanda's screenshot](https://imgur.com/FJxpOzx)
- [Jason's screenshot](https://imgur.com/l8ULZAX)
- [Wayne's screenshot](https://imgur.com/zHGcMUC)

## Instructions to execute (Only those with NUID can access)
1. `git clone` current project
2. `cd` to current file
3. `chmod +x webcrawler`
4. `./webcrawler` username password

## Contributors
[Amanda Au-Yeung](https://github.com/amandaay), [Jason Chen](https://github.com/JasonKTChen) , [Wayne Tseng](https://github.com/Chun-Wei-Tseng)

