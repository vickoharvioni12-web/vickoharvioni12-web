import base64

# Open the original image uploaded by user in prompt 1
with open('download.jpg', 'rb') as f:
    img_data = f.read()

b64_str = base64.b64encode(img_data).decode('utf-8')
data_uri = f"data:image/jpeg;base64,{b64_str}"

# Print length check
print("Base64 string length:", len(data_uri))

# Create full markdown code using Base64 URI so it NEVER breaks or needs upload
readme_content = f"""<div align="center">

  <!-- BANNER PIXEL ART SAMUDRA (BASE64 INLINE - PASTI MUNCUL TANPA UPLOAD) -->
  <img src="{data_uri}" alt="Vicko Harvioni Pixel Ocean Banner" width="100%" style="border-radius: 8px;" />

  <br/><br/>

  <h1>🌊 Hi there, I'm Vicko Harvioni! 👋</h1>
  <p><b>Web Developer | Node.js & Python Specialist | Linux Enthusiast</b></p>

  <!-- TECH STACK BADGES -->
  <p>
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  </p>

</div>

---

### 🚀 About Me

```bash
$ cat vicko_harvioni.txt
> Hi! I'm Vicko Harvioni — a Web Developer focused on building clean and efficient applications.
> Primary focus: Node.js backend, Python automation, modern Web Development, and Linux.
> Always exploring new technologies like diving into the deep ocean 🌊.
