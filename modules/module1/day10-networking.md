# Module 1 — Day 10: Basic Networking Lab (Packet Tracer)

## 🎯 Objectives
- Understand how to view listening services and open ports.
- Learn how processes bind to TCP/UDP sockets.
- Tie networking basics into **cloud & security** use cases.

---

## 🔎 Commands

### 1. Show listening ports
```bash
ss -tulnp
# or
netstat -tulnp
sudo lsof -i -P -n | grep LISTEN
ss -tulnp | grep ssh
sudo tcpdump -i any port 53 -nn -c 10
tcp   0   0 127.0.0.1:39549     0.0.0.0:*    LISTEN   78826/rootlesskit
tcp   0   0 127.0.0.53:53       0.0.0.0:*    LISTEN   512/systemd-resolve
tcp6  0   0 :::22               :::*         LISTEN   1/init
udp   0   0 0.0.0.0:5353        0.0.0.0:*             822/avahi-daemon: r
