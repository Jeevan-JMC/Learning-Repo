## Jenkins Installation on Ubuntu (Step-by-Step)

### Step 1: Install Java (Required by Jenkins)

Jenkins requires Java to run. We'll install **OpenJDK 21**.

```bash
sudo apt update
sudo apt install fontconfig openjdk-21-jre
```

✅ Verify the Java version:

```bash
java -version
```

You should see something like:

```
openjdk version "21.0.3" 2024-04-16
OpenJDK Runtime Environment (build 21.0.3+11-Debian-2)
OpenJDK 64-Bit Server VM (build 21.0.3+11-Debian-2, mixed mode, sharing)
```

📘 *Official Jenkins requirements page:*
👉 [https://www.jenkins.io/doc/book/installing/linux/](https://www.jenkins.io/doc/book/installing/linux/)

---

### Step 2: Install Jenkins

1. **Add Jenkins GPG key:**

```bash
sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2026.key
```

2. **Add Jenkins repository:**

```bash
echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```

3. **Install Jenkins:**

```bash
sudo apt-get update
sudo apt-get install jenkins -y
```

---

### Step 3: Start and Check Jenkins

Check if Jenkins is running:

```bash
sudo systemctl status jenkins
```

To start Jenkins (if not already running):

```bash
sudo systemctl start jenkins
```

---

### Step 4: Access Jenkins Web UI

* Open your browser and go to:
  `http://<YOUR_PUBLIC_IP>:8080`

* You will be asked for an **initial admin password**. Retrieve it using:

```bash
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

---

### ⚠️ Important Notes (Cloud Environment)

* Ensure **port 8080** is open in your cloud firewall settings.
* You can set this in **GCP, AWS, Azure** as per your VM’s configuration.

---

📘 *Official Jenkins installation guide:*
👉 [https://www.jenkins.io/doc/book/installing/linux/](https://www.jenkins.io/doc/book/installing/linux/)

---

