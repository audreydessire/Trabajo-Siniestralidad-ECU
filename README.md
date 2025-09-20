# Siniestralidad ECU — Reproducibilidad

Este repositorio contiene el cuaderno Jupyter para modelado **SARIMA** y generación de pronósticos de siniestralidad en Ecuador.

> **Reproducibilidad**: las dependencias están **fijadas** en `requirements.txt`.  
> **Versión de Python requerida:** **3.10.11**.

---

## 📥 Clonar el repositorio

Para obtener el código en tu máquina:

```bash
git clone https://github.com/audreydessire/Trabajo-Siniestralidad-ECU.git
cd Trabajo-Siniestralidad-ECU
```

---

## 🐍 Instalar Python 3.10.11

Este proyecto requiere **Python 3.10.11**.

### 🔹 Windows
1. Descarga el instalador oficial desde:  
   👉 [Python 3.10.11 - Windows Installer (64-bit)](https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe)  
2. Ejecuta el instalador marcando la casilla **"Add Python to PATH"**.  
3. Verifica la instalación:
   ```bash
   python --version
   # Debe mostrar: Python 3.10.11
   ```
---

## 📁 Estructura del proyecto

```
.
├─ Siniestralidad ECU.ipynb
├─ siniestro_info_mercado_ecuador.xlsx   # fuente de datos usada en el notebook
└─ requirements.txt                      # dependencias con versiones fijas

```


## ✅ Requisitos

- **Python 3.10.11**
- `pip` ≥ 22
- VS Code (recomendado) con extensiones **Python** y **Jupyter**

### Comprobar tu Python
```bash
python --version
# Debe mostrar: Python 3.10.11
```

## 🚀 Instalación rápida

### Windows (PowerShell / Terminal de VS Code)
```powershell
py -3.10 -m venv .venv_arima
.\.venv_arima\Scripts\activate
pip install -r requirements.txt
```

## 🧠 Seleccionar el kernel en VS Code

1. Abre `Siniestralidad ECU.ipynb`.
2. En la esquina superior derecha, haz clic en el selector de kernel.
3. Elige **`.venv_arima (Python 3.10.11)`**.  
   (Si no aparece, abre la paleta `Ctrl+Shift+P` → **Python: Select Interpreter** →  
   **Enter interpreter path** → busca `./.venv_arima/Scripts/python.exe`).


---

## ▶️ Ejecutar

- Con el entorno activado y el kernel seleccionado, abre el notebook y pulsa **Run All**.
- El cuaderno:
  - carga el Excel `siniestro_info_mercado_ecuador.xlsx`,
  - ajusta el modelo SARIMA,
  - muestra métricas/diagnósticos,
  - y genera pronósticos (12 pasos por defecto).

---


## 🧩 Dependencias principales

(Están fijadas en `requirements.txt`; aquí lo esencial del proyecto)

- `pandas==2.2.2`, `numpy==1.26.4`, `openpyxl==3.1.5`
- `matplotlib==3.8.4`, `seaborn==0.13.2`
- `statsmodels==0.14.2`, `scikit-learn==1.4.2`, `scipy==1.11.4`
- `pmdarima==2.0.4`
- `ipykernel==6.30.1` (kernel Jupyter para el venv)

