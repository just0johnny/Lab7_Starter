# Lab 7 Question Answers

Johnny Huang

## Question 1

Q: Where would you fit your automated tests in your Recipe project development pipeline?

A: The best choice is 1, since putting tests into GitHub Actions would make the tests run every time the code is pushed, which is ideal since it would force testing everytime without fail.

## Question 2

Q: Would you use an end to end test to check if a function is returning the correct output? (yes/no)

A: No, checking a function is more of a unit test.

## Question 3

Q: What is the difference between navigation and snapshot mode?

A: The difference between navigation and snapshot mode is that navigation mode analyzes the page after it (re)loads. This allows it to score the performance of the loading, but it won't be able to analyze changes beyond the starting page after loading. Snapshot mode, on the other hand, analyzes the page without reloading it, so the current state that it is in. This helps in analyzing the page in specific states, particularly accessibility issues.

## Question 4

Q: Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

A:
1. For accessibility: it states "<html> element does not have a [lang] attribute", which I believe states the language of the page, so to include that would improve accessibility.
2. LCP Breakdown: it states that most of the LCP time should not be spent on delays, but rather loading the resources (the element render delay is 26,280 ms in this case, which seems too high), so reducing the delay would improve the time.
3. Network Dependency Tree: it states to avoid chaining critical requests to improve page load, which the path there takes 569 ms, with options like reducing the length of the chains, this would improve load time as well.