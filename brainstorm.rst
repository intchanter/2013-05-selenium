Topics to cover:

- What is Selenium?
  - A tool for driving a browser as if a user were using it
  - Can drive Firefox, Chrome, Safari, IE
- Why use page maps?
- Why use page objects?
- Which selector type to favor? (CSS)
  - xpath is less maintainable, more likely to change as work progresses on the pages
  - css is more popular
  - css takes less typing on average
  - css is more broadly understood
  - historically, there were significant performance differences with IE
- Explicit vs. implicit waits


│19:04:30        llaskin1 | "and after you have realized how awesome
│                         | Selenium is, get yourself involved with the
│                         | community, hop int he chatroom, submit
│                         | patches, fix bugs, file bugs ,etc"

Demonstrations:
- Start a browser
- Open a web page
- Find an element on the page using each of the different types of selectors
- Use an implicit wait
- Use an explicit wait
- Use a page map
- Use a page object
- CSS refresher
- XPATH quick overview
- Cleaning up

Story:
- Introduce Alice and Bob
  - Alice needs to get data from a site, but they don't provide an API
  - Bob needs to test a web application
- Enter Selenium!
  - Bob uses Selenium to test the web application Firefox, Chrome, and IE
  - Alice uses Selenium to drive a PhantomJS browser instance to get her data
- Uh, oh, something changed!
  - The web developers changed the css selectors Bob used in his tests!
  - Now he needs to go through and change the selectors everywhere
- DRY review
- Enter page maps
  - Bob uses a key-value data type to store the selectors he needs, separating the way their code accesses the page from the way the page is constructed
  - Now he only need to update the page map structure when something changes
  - He tells Alice, and she starts doing the same thing to address a similar issue
- Something bigger changed!
  - Alice needs more data, but the steps to get the data have changed
- Enter page objects
  - Alice creates a class for each unique page and puts the page maps in them
  - Alice adds object methods corresponding to specific tasks to be done
  - Now if something changes again, she only needs to update the page object
- Alice and Bob get involved in the community
  - IRC
  - Github/Google Code
  - Mailing list
- Finding more information
  - Official project documentation
  - Twitter
  - Blogs
  - Language binding documentation
  - StackOverflow
