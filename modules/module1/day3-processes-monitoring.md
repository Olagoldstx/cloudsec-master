# Module 1 — Day 3: Processes & System Monitoring

## Objectives
- Learn to view and manage processes
- Monitor CPU, memory, and services
- Explore system logs

## Commands
```bash
ps aux | head -10
top
htop
systemctl status ssh
journalctl -xe

---

### Day 4 — Package Management
```markdown
# Module 1 — Day 4: Package Management

## Objectives
- Learn how to install, update, and remove software
- Understand package repositories and security updates

## Commands
```bash
sudo apt update
sudo apt upgrade
apt list --installed
sudo apt remove package-name

---

### Day 5 — Bash Scripting Basics
```markdown
# Module 1 — Day 5: Bash Scripting Basics

## Objectives
- Write simple shell scripts
- Use variables, loops, and conditionals
- Automate common tasks

## Commands
```bash
nano hello.sh
echo "echo Hello, Cloud Security" > hello.sh
chmod +x hello.sh
./hello.sh

---

### Day 6 — Users & Groups Deep Dive
```markdown
# Module 1 — Day 6: Users & Groups Deep Dive

## Objectives
- Explore `/etc/passwd`, `/etc/group`
- Create and manage users & groups
- Understand UID/GID roles

## Commands
```bash
cat /etc/passwd | head -5
cat /etc/group | head -5
sudo adduser analyst
sudo groupadd secops
sudo usermod -aG secops analyst

---

### Day 7 — Filesystems & Disk Usage
```markdown
# Module 1 — Day 7: Filesystems & Disk Usage

## Objectives
- Understand disk layout and mounts
- Monitor usage with `df` and `du`
- Edit `/etc/fstab` for persistence

## Commands
```bash
df -h
du -sh *
mount
lsblk

---

### Day 8 — Logs & Log Security
```markdown
# Module 1 — Day 8: Logs & Log Security

## Objectives
- Explore `/var/log/`
- Learn `journalctl` basics
- Configure log rotation

## Commands
```bash
ls -l /var/log
journalctl -p err -n 20
cat /var/log/auth.log

---

### Day 9 — Firewall Basics
```markdown
# Module 1 — Day 9: Firewall Basics

## Objectives
- Learn UFW basics
- Allow/deny traffic
- Check active rules

## Commands
```bash
sudo ufw enable
sudo ufw allow 22
sudo ufw deny 80
sudo ufw status
