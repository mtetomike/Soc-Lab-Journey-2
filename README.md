# Threat Hunting and Log Detection


# 🔎 Threat Hunting & Log Detection

## 🎯 Objective
Practice identifying suspicious behavior using Linux logs and system monitoring tools.

---

## 🛠 Tools Used

- journalctl
- cat /var/log/auth.log
- grep
- ss -tnp
- ps aux
- top

---

## 🚨 Scenarios Investigated

1. Multiple failed SSH login attempts
2. Suspicious high CPU process
3. Unexpected outbound network connection
4. Unauthorized sudo usage

---

## 🔍 Example Detection

### Failed Logins

```bash
grep "Failed password" /var/log/auth.log
ps aux --sort=-%cpu

