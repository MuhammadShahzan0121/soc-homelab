# Network Setup

## Objective

Configure communication between Ubuntu and Windows virtual machines in VMware Fusion.

---

## VMware Fusion Network Configuration

Both virtual machines were configured using:

* Share with my Mac (NAT)

This allowed:

* Internet connectivity
* Communication between virtual machines

---

## Ubuntu SIEM Server

IP Address:
192.168.33.129

Command Used:

```bash id="pq9l09"
ip a
```

Screenshot:
<img width="742" height="561" alt="ubuntu-ip-address" src="https://github.com/user-attachments/assets/1867b138-4c87-4bab-af1c-5085060dc0f4" />


---

## Windows Endpoint

IP Address:
192.168.33.130
Command Used:

```powershell id="xgrv7y"
ipconfig
```

Screenshot:
<img width="738" height="563" alt="windows-ip-address" src="https://github.com/user-attachments/assets/42eccccb-099b-4b76-82f5-8674c2813106" />


---

## Connectivity Testing

Ping testing confirmed communication between both virtual machines.

Command Used:

```powershell id="6ib7uo"
ping <192.168.33.129>
```

Result:
Successful replies received.

Screenshot:
<img width="539" height="281" alt="ping-test-success" src="https://github.com/user-attachments/assets/1cc960b2-afab-4b9d-a880-cedb40bfb3da" />

---

## Lessons Learned

* SIEM platforms require reliable network communication.
* VMware Fusion NAT networking simplifies virtual machine connectivity.
* Basic networking skills are essential for cybersecurity labs.
