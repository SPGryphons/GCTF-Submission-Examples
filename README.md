Challenge Submission Template 
===

## Flag Format
- `GCTF23{...}`

## Submission Guide

### Option 1: CTF-Architect (Preferred)
- [CTF-Architect](./CTF-Architect/) is a tool that currently supports the creation & templating of challenges created for the Gryphons CTF. 
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


## Navigation
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