## Lab 12

- Name:
- Email

## Part 1 Answers:

1. `tar` options:
   - `-c` Compress an entire directory
   - `-v` verbose output
   - `-f` use archive file
   - `-z` create gzip archive
   - `-x`extract an archive
2. Command(s):tar -czvf file.tar.gz Lab10

## Part 2 Answers:

1. Command:
2. `sftp` options:
   - `ls` lists all files in foreign directory
   - `lls` lists all files in home directory
   - `put` upload file
   - `get` download file 
3. Command(s): get file.tar.gz
4. Command(s): tar -xzvf file.tar.gz

## Part 3 Answers:

1. sudo adduser testguy
2. ssh-keygen
3. "put testkey" in sftp then move it to correct folder
4. ssh -i testkey testguy@44.211.102.140

## Part 4 Answers

1. Translate to network prefixes + CIDR notation:
   - Sample: `10.0.0.0 - 10.0.1.255` = `10.0.0.0/23` OR `10.0.1.0/23`
   - `130.108.0.0 - 130.108.255.255` = 130.108.0.0/16
   - `10.0.0.0 - 10.0.0.255` = 10.0.0.0/24
   - `your_public_ip - your_public_ip` = 130.108.220.1/24
2. How you confirmed current rules are bad, and why are they bad. Sudo iptables -L. It can allow malicious connections.
3. Your implementation details and **screenshot** removed all port connections that were not 22 https://imgur.com/a/reU5EXp
4. Something invalid: ubuntu@44.211.102.140

## Extra Credit Answers:

### Solve the conflict

1.
2.
3.
4.
5.
