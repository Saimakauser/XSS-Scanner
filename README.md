# XSS-Scanner
A Python-based automated XSS (Cross-Site Scripting) vulnerability scanner that detects reflected XSS vulnerabilities by extracting HTML forms from a target website, injecting a JavaScript payload into input fields, and analyzing the server response.

This tool helps understand how reflected XSS attacks work and how web applications can be tested for basic input validation flaws.

🚀 Features

Automatically extracts all forms from a target URL

Identifies form action, method (GET/POST), and input fields

Injects a custom JavaScript payload into text and search inputs

Submits forms dynamically using GET or POST requests

Detects reflected XSS by checking response content

Displays vulnerable form details using structured output

🛠 Technologies Used

Python 3

requests – For sending HTTP requests

BeautifulSoup (bs4) – For parsing HTML and extracting forms

urllib.parse (urljoin) – For handling relative form action URLs

pprint – For structured display of vulnerable form details

⚙ How It Works

The scanner fetches the webpage content.

Extracts all <form> elements from the HTML.

Collects form details (action, method, input fields).

Injects a JavaScript payload into text/search inputs.

Submits the form to the target server.

Checks whether the payload appears in the response.

If detected, it reports the form as vulnerable to reflected XSS.

⚠ Disclaimer

This tool is developed strictly for educational and ethical testing purposes. Do not use it on websites without proper authorization.
