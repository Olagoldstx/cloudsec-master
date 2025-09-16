# Module 1 — Day 1: Linux Shell Basics (Expanded)

## Concepts
- Filesystem: `pwd`, `ls -lah`, `cd`, `mkdir`, `cat`
- Users/permissions: `whoami`, `id`, `chmod +x`
- Redirection/pipes: `>`, `>>`, `| grep`
- Processes/jobs: `ps aux`, `top`, `sleep 100 &`, `jobs`, `kill %1`
- Packages: `sudo apt update`, `sudo apt install htop`
- Networking: `ping -c 4 google.com`, `curl -I https://example.com`
- Monitoring: `df -h`, `du -sh *`, `free -h`, `uptime`

## Labs (what to expect)
- Ping shows 0% loss; curl returns `HTTP/2 200`
- `chmod +x` adds execute bit
- `jobs` lists background tasks; `kill` stops them

## Deep Reasoning Analogy
Linux is a **warehouse**; the shell is your **forklift controller**. These basics make the later Terraform/Kubernetes/PCNSE labs intuitive.
