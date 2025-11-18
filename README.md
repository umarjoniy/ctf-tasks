# CTF Challenge Development Task

This is CTF tasks created for educational purposes during my internship period.

For solution, please approach **solution.md** file.

## "Command Injection"
- Difficulty: **hard**
- Topics: Code Injection
- Inspiration: Hack The Box Academy, Code Injection module, Skills Assessment section

Setup: `sudo docker build -t code_injection . && sudo docker run code_injection`

## "SSRF"
- Difficulty: **medium**
- Topics: SSRF
- Inspiration: Hack The Box Academy, Server-Side Attacks, SSRF sections

Setup: `sudo docker-compose build & sudo docker-compose up -d`

To Stop: `sudo docker-compose down -v --remove_orphans`

## "Think Outside of the Box"
- Difficulty: **easy**
- Topics: Creativity, bypass regex domain filter to point into localhost
- Inspiration: fun

Setup: `sudo docker build -t easy . && sudo docker run easy`
