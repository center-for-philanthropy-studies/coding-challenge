# CEPS Coding Challenge - Webscraping 💻
This is a small challenge set for all applicants that would like to apply to [this open position at CEPS](https://jobs.unibas.ch/offene-stellen/junior-developer-hilfsassistent-in/97f174ac-fc53-4726-8f29-f158e899a46f?utm_campaign=google_jobs_apply&utm_source=google_jobs_apply&utm_medium=organic). It is a simple webscraping task that we already implemented. So it is a real use case, and it is not only for us to see how you approach problems, but also for you to get an idea what kind of problems you can expect. 

### Scrape Email Adresses
The goal of this challenge is to write a simple script that scrapes email-addresses of a given entity (this could be a company, foundation, NGO or any other kind of organization). All information given is the name of the entity.

### Tasks
1. Write a function that takes the entity name as an input, then runs a webscraper algorithm that looks out for email-addresses of that entity and returns the findings as an array (or empty array/null if nothing was found). If you find multiple addresses, gather all of them.
2. The webscraping algorithm could be something like this (PSEUDO CODE): 
```ruby
def scrape_emails(entity_name)
  # SCRAPE ALGORITHM PSEUDO CODE
  # 1. open webbrowser
  # 2. google the entity_name
  # 3. when google returns results, open the first result
  # 4. extract all email addresses from this website
  # OPTIONAL: if no email address is found in previous step, search for a contacts page, click on it, and redo step 4.
  # return emails as array
end
```
3. If you have a function that works for a single entity name, write a script where you iterate over a list of entity names, scrape them and store the results in a file of your choice (JSON, csv, XML, ...). Use the files described in the next section as inputs.

### Data
This repo contains two files:
- **`entity_names_example.txt`**: In this file you find 3 entities to test your algorithm. They are manually selected and should be easy to scrape.
- **`entity_names_example_SOLUTION.txt`**: here you will find the emails your scraper should find for all 3 examples. You can use this to check if your scraper works.
- **`entity_names_real.txt`**: This is real data we used for this scraping task. Our hitrate for these entities is around 30-40%. You don't need to run it, but if you are curious and have a working algorithm you can totally run your script with this real data and send the results, would be interesting to discuss the differences. 

### Rules
1. **any language and any scraping framework is allowed**: but it's a plus if you use [**`ruby`**](https://www.ruby-lang.org/de/) and [**`selenium`**](https://rubygems.org/gems/selenium-webdriver/versions/2.53.0?locale=de), since this is the stack we are working with. 
2. the script does not have to be perfect. Webscraping is never accurate, there will be always noise and wrongly classified data, especially when you run the real data example.
3. If you have any questions, please ask. I can help you with setting up selenium and ruby if thats a challenge. Also if you need some ideas or are stuck with a problem, don't hesitate to contact me via mail (thomas.starzynski@unibas.ch).
4. There is no time limit to this task, but ideally you can implement it in 4-6h. 

**HAPPY SCRAPING** 🚀
