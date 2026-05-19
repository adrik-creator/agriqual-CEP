# 🌿 AgriQualStat — Control Estadístico de Calidad

**Universidad del Magdalena · CEP 2026-1**  
Frutas, Hortalizas y Plantas Medicinales

---

## ¿Qué incluye?

| Herramienta | Descripción |
|---|---|
| Gráficos X̄-R y X̄-S | Variables continuas con constantes d₂, A₂, A₃, B₃, B₄, D₃, D₄ |
| Gráficos p, np, c, u | Control de atributos con límites automáticos |
| Cp, Cpk, Pp, Ppk | Índices de capacidad del proceso |
| Diagrama de Pareto | Análisis 80/20 de defectos |
| Shapiro-Wilk + Anderson-Darling + K-S | Pruebas de normalidad |
| Q-Q Plot + Histograma | Visualización de normalidad |
| Estadísticas descriptivas | Media, varianza, std, CV, asimetría, curtosis |
| Trazabilidad | Producto, analista, fecha, lote |
| Exportar Excel | Resultados descargables |

---

## 🚀 Cómo publicar GRATIS en Streamlit Cloud (compartible con enlace)

### Paso 1 — Subir a GitHub
1. Crea una cuenta en [github.com](https://github.com) si no tienes.
2. Crea un repositorio nuevo (público), ej: `agriqual-cep`.
3. Sube los dos archivos:
   - `app.py`
   - `requirements.txt`

### Paso 2 — Publicar en Streamlit Cloud
1. Ve a [share.streamlit.io](https://share.streamlit.io) e inicia sesión con GitHub.
2. Clic en **"New app"**.
3. Selecciona tu repositorio `agriqual-cep`.
4. En **"Main file path"** escribe: `app.py`
5. Clic en **"Deploy!"**

En 2-3 minutos tendrás un enlace como:  
`https://tu-usuario-agriqual-cep.streamlit.app`

¡Ese enlace lo puedes compartir con cualquier persona sin que instalen nada!

---

## 🖥️ Correr localmente

```bash
pip install -r requirements.txt
streamlit run app.py
```

Abre tu navegador en `http://localhost:8501`

---

## 📋 Formato de datos Excel

**Variables continuas:**  
Cada fila = un subgrupo. Cada columna = una medición.
```
12.3 | 12.1 | 12.5 | 11.9 | 12.4   ← Subgrupo 1
11.8 | 12.2 | 12.0 | 12.3 | 11.7   ← Subgrupo 2
```

**Atributos:**  
Una columna con el conteo por subgrupo.
```
3
5
2
7
4
```

**Pareto:**  
Dos columnas: Defecto | Cantidad
```
Manchas    | 45
Plagas     | 30
Golpes     | 20
```
