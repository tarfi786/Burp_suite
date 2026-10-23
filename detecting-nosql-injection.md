# Detecting NoSQL injection

**Platform:** PortSwigger Web Security Academy  
**Status:** In progress — not solved at last check  
**Last checked:** 2026-10-23

## Objective

Practice identifying and analyzing potential NoSQL injection behavior in the designated training lab.

## Environment

- Tool: Burp Suite Community Edition
- Browser: Google Chrome
- Target: The assigned PortSwigger Academy lab instance
- Authorization: Training lab only

## Workflow

1. Open the assigned lab instance.
2. Use Proxy → HTTP history to locate the relevant category-filter request.
3. Send the request to Repeater.
4. Keep a copy of the baseline request and response.
5. Change only one input at a time, using the lab's instructions and safe test cases.
6. Compare status codes, response content, and error messages.
7. Record the exact result observed.
8. Stop and revisit the lab instructions if the response is ambiguous or produces a server error.
9. Mark the lab solved only after the Academy page confirms success.

## Observations

- A request using a category parameter was observed.
- Some modified inputs produced HTTP 500 responses with JavaScript syntax errors.
- One modified input returned HTTP 200, but that alone did **not** establish that the lab was solved.
- The lab page showed **Not solved** in the available screenshot.

## Results

**Not solved at last check.** No claim of successful exploitation is made here.

## Lessons learned

- A `200 OK` response does not automatically mean a test succeeded.
- Server errors are observations, not proof of a vulnerability by themselves.
- Preserve a baseline request and make one change at a time.
- Verify the lab's explicit success condition.

## Evidence

Add sanitized screenshots to `../screenshots/` and reference them here only after checking that they contain no cookies, tokens, personal information, or other sensitive data.
