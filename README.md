# ROCm PyTorch Jupyter Notebook Template

A minimal template for running **PyTorch with ROCm support** inside a **Dockerized Jupyter Notebook** environment.  
This setup is designed to give you a ready-to-use workspace for machine learning and deep learning projects.

---

## 🚀 Features
- **ROCm-enabled PyTorch** for AMD GPUs  
- **Jupyter Notebook** interface for interactive development  
- **Dockerized setup** with `docker-compose` for easy start/stop  
- An `app/` folder where your project code and notebooks live  

---

## 📂 Project Structure
```

.
├── app/                # Your notebooks and project files go here
├── Dockerfile          # Defines the PyTorch + Jupyter + ROCm environment
├── docker-compose.yml  # Orchestrates the service

````

---

## 🛠️ Requirements
- Docker
- Docker Compose
- AMD GPU with ROCm support  

---

## ▶️ Usage

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Nontre12/docker-rocm-pytorch-jupyter
   cd docker-rocm-pytorch-jupyter
   ```

2. **Start the service:**

   ```bash
   docker-compose up --build
   ```

3. **Access Jupyter Notebook:**
   Open [http://localhost:8888](http://localhost:8888) in your browser.
   The token will be shown in the container logs.

4. **Place your work in the `app/` folder.**
   Notebooks and code inside `app/` will be available inside Jupyter.

---

## 📌 Notes

* This template assumes you have ROCm drivers installed on your host system.
* Modify the `Dockerfile` if you want to add extra dependencies (e.g., TensorBoard, SciPy stack).
* Data volumes can be mounted in `docker-compose.yml` if needed.

---

## 📜 License

MIT License
