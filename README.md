# pipe-flow-analysis-tool
A Python-based process engineering tool for hydraulic calculations, including velocity, Reynolds number, friction factor, Darcy-Weisbach pressure losses, and local losses. The tool provides step-by-step equations and generates professional PDF reports with full calculation transparency.

Engineering tool developed in Python for pipe flow and hydraulic analysis.  
It performs key process calculations and generates professional PDF reports with full equation transparency.

---

## 🚀 Features

- Pipe flow velocity calculation
- Reynolds number determination
- Flow regime classification (Laminar / Turbulent)
- Friction factor estimation
- Darcy-Weisbach pressure loss calculation
- Local losses (valves, elbows, fittings)
- Static head contribution
- Total system pressure calculation
- Step-by-step calculation breakdown (engineering transparency)
- PDF report generation with:
  - Company logo
  - Structured layout
  - Full equations and results

---

## 🧠 Engineering Approach

This tool was built with a strong focus on **engineering clarity and validation**.

Instead of only providing results, it shows:

- Equations used in each step
- Intermediate values
- Final results in engineering units

This allows:
- Easier validation by other engineers
- Better understanding of the process
- Use in real engineering discussions

---

## 📐 Equations Used

### Flow Velocity
v = Q / A

### Reynolds Number
Re = (ρ · v · D) / μ

### Friction Factor
- Laminar: f = 64 / Re  
- Turbulent: f ≈ 0.02 (approximation)

### Darcy-Weisbach
hf = f · (L/D) · (v² / 2g)

ΔP = ρ · g · hf

### Local Losses
ΔP = K · (ρ · v² / 2)

### Static Head
ΔP = ρ · g · H

---

## 🖥️ Interface

- Simple and intuitive GUI (Tkinter)
- Input fields for:
  - Pipe diameter
  - Flow rate
  - Fluid properties
  - Pipe length
  - Fittings and valves
  - Extra losses
  - Static head

---

## 📄 PDF Report

The tool automatically generates a professional report including:

- Logo (custom upload)
- Organized sections
- Engineering calculations
- Step-by-step equations

---

## ⚙️ Requirements

Install dependencies:

```bash
pip install reportlab
