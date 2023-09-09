Challenge Submission Template 
===

## Flag Format
- `GCTF23{...}`

## Submission Guide

### Option 1: CTF-Architect (Preferred)
- [./CTF-Architect/](https://github.com/Jus-Codin/CTF-Architect/) is a tool that currently supports the creation & templating of challenges created for the Gryphons CTF. 
- Do note that this tool is still in development, and may not be fully functional. If you encounter any issues, please contact the Gryphons team for assistance.

##### 1. Clone this Git Repository
```bash
git clone https://github.com/SPGryphons/GCTF-Submission-Examples
```
#### 2. Install CTF-Architect
```bash
cd ./GCTF-Submission-Examples/CTF-Architect
python -m pip install .
```
#### 3. Ensure CTF-Architect is installed
```bash
ctf-architect --help
chall-architect --help
```

#### 4. Start packaging your challenge
```bash
chall-architect
```

![1](https://i.imgur.com/WYZeZV3.png)
![2](https://i.imgur.com/OCjMhEf.png)

#### 5. Submit your challenge
- If everything goes well, your challenge should be packaged & templated nicely in the folder specified.
- You can now **zip** the folder and submit it in the google form provided.

### Option 2: Manual Submission (not recommended)
- If you are unable to use CTF-Architect, you may manually submit your challenge.
- Please follow the template provided in the [templates](./template) directory.
- Do note that minor errors in the template may result in the challenge breaking, in such cases we may contact you for clarification, examples of working challenges can be found in the [examples](./examples) directory.

## Navigation
- [CTF-Architect](./CTF-Architect)
    - Contains the CTF-Architect tool for challenge packaging & templating
- [examples](./examples)
    - Contains challenge documentation examples for OSINT, Static & Hosted Web Challenges
- [templates](./templates)
    - Contains the challenge submission templates challenge submission, please follow the template.

## Additional Notes
- Failure to follow the template will most likely result in the rejection of your challenge, however you may be contacted for clarification if necessary.
- Any questions or concerns can be directed to the #ticket-support channel on the [Gryphons Discord Server](https://discord.gg/2nZTCdBGgY)

## Frequently Asked Questions
- **Q:** What do I do if I don't know how to write a `Dockerfile` for **web** challenges?
    - **A:** The preferred method is to refer to provided [Dockerfiles](./examples/web/Hello,%20Cookie%20Monster/service/hello-cookies/Dockerfile) in the [examples](./examples) directory. If you are still having trouble, please contact the Gryphons team for assistance.
- **Q:** How do I submit a **pwn/re** challenge?
    - **A:** As the architecture & infrastructure is yet to be confirmed, pwn & re challenges will be compiled by the Gryphons team. Please ensure that the compiler flags & specific compilation instructions are provided in the challenge documentation.
    - e.g `gcc -o challenge challenge.c -fno-stack-protector -z execstack -no-pie`
    - Challenges that include a pre-compiled binary are expected to have source code provided, and will be recompiled by the Gryphons team.
    - A sample Dockerfile for a standard ret2win challenge can be found here: [Dockerfile](./examples/pwn/Alien%20Portal/service/alien_portal/Dockerfile)
- **Q:** My challenge has custom/non-standard hosting requirements, what do I do?
    - **A:** Please contact the Gryphons team for assistance, we will try our best to accommodate your requirements.
