# Module 1 — Day 2: Permissions & sudo Security

## Concepts
- **Users & Groups**: `whoami`, `id`, `groups`, `adduser`, `usermod -aG`
- **Permissions**: `ls -l`, read (r), write (w), execute (x)
- **Change Ownership**: `chown`, `chgrp`
- **Change Mode**: `chmod 644 file.txt`, `chmod +x script.sh`
- **umask**: default file permissions
- **Sudo & /etc/sudoers**: privilege escalation, least privilege

## Deep Reasoning Analogy
Think of your Linux system as a **castle**:
- Users = villagers
- Groups = guilds
- Permissions = keys to doors
- sudo = the king's special seal (only trusted knights)

## Commands to Try
\`\`\`bash
# 1. See who you are
whoami
id
groups

# 2. Inspect permissions
ls -l /etc/passwd
ls -ld /home

# 3. Change permissions (lab will create the files first)
touch secret.txt
chmod 600 secret.txt   # owner rw only
ls -l secret.txt

# 4. Add execute
echo "echo Hello" > script.sh
chmod +x script.sh
./script.sh

# 5. Ownership (requires sudo)
sudo chown root:root secret.txt

# 6. Sudo
sudo whoami
\`\`\`

## Lab: Sudo Security
1. Add a new user:
   \`\`\`bash
   sudo adduser tester
   \`\`\`
2. Try \`sudo whoami\` (as tester) — should fail.
3. Add tester to sudo group:
   \`\`\`bash
   sudo usermod -aG sudo tester
   \`\`\`
4. Switch user and test:
   \`\`\`bash
   su - tester
   sudo whoami
   \`\`\`

## Checklist
- [ ] Run whoami and id
- [ ] Practice chmod (600, 644, +x)
- [ ] Practice chown and chgrp
- [ ] Create/test a sudo user
