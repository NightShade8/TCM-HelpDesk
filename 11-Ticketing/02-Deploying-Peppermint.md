# 🚀 Deploying Peppermint Using Docker

## 🛠️ Steps to Deploy
1. **Install Docker** on your system if not already installed.
2. **Pull the Peppermint Docker image**:
    ```bash
    docker pull peppermint/ticketing
    ```
3. **Run the container**:
    ```bash
    docker run -d -p 8080:80 --name peppermint peppermint/ticketing
    ```
4. **Access Peppermint** via browser:
    ```
    http://localhost:8080
    ```

---

## 🔧 Managing Peppermint with Docker
| **Command**                 | **Description**              |
|-----------------------------|-----------------------------|
| `docker stop peppermint`    | Stop the container.         |
| `docker start peppermint`   | Restart the container.      |
| `docker rm peppermint`      | Remove the container.       |

---

## 📚 Summary
Deploying Peppermint via Docker enables **fast setup and management** for effective ticketing.
