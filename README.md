# 🛡️ Task 3 - Perform a Basic Vulnerability Scan on Your PC.

## 🔧 Tool Used
- **Nikto v2.5.0**
- Installed via **Homebrew** on macOS

## 🖥️ Target
- Localhost: `http://127.0.0.1:8080`
- Server: **Jetty 12.0.19** running Jenkins

## 🛠️ Scan Command
```bash
nikto -h http://127.0.0.1:8080
```

## 📄 Summary of Findings
- ❌ Missing `X-Frame-Options` header
- ❌ Missing `X-Content-Type-Options` header
- 🔍 Server identifies as Jenkins via uncommon headers and favicon
- 🧭 CGI directories detected

## 📁 Output File
See: [`nikto_result.txt`](nikto_result.txt)
