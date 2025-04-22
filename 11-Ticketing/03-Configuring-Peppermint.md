# 📌 Configuring Peppermint on Linux

## 🛠️ Installing Peppermint on Linux
1. **Update your system**:
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```
2. **Install dependencies**:
    ```bash
    sudo apt install docker docker-compose -y
    ```
3. **Pull and run the Peppermint Docker container**:
    ```bash
    docker run -d -p 8080:80 --name peppermint peppermint/ticketing
    ```
4. **Access Peppermint** via browser:
    ```
    http://localhost:8080
    ```

---

## ⚙️ Configuring Peppermint
1. **Set up Admin Credentials** (follow on-screen instructions).
2. **Configure Email Notifications** (SMTP settings in the admin panel).
3. **Create User Roles** (Admin, Support, User).
4. **Customize Ticket Categories** (IT Support, Network Issues, Software Requests, etc.).
5. **Enable Logging & Backup** for better tracking.

---

## 🔧 Managing Peppermint
| **Command**                 | **Description**              |
|-----------------------------|-----------------------------|
| `docker restart peppermint` | Restart Peppermint.         |
| `docker logs peppermint`    | Check container logs.       |
| `docker stop peppermint && docker rm peppermint` | Stop and remove the container. |

---

## 📚 Summary
Configuring Peppermint ensures **efficient ticket management**, customizable workflows, and secure authentication.
