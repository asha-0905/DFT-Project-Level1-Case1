# DFT-Project-Level1-Case1

This project demonstrates **Design-for-Testability (DFT) Scan Insertion** on a sample sequential design using Mentor Graphics **Tessent Shell**.  
The goal was to identify non-scan flops, replace them with scan-enabled cells, and create balanced scan chains.

---

## 🚀 Flow Summary

1. **Read Design & Library**
   - Loaded RTL/netlist (`case1_man_fix.v`)
   - Linked with TSMC13 standard cell library

2. **DFT DRC Checks**
   - Identified 40 sequential flops
   - Reported non-scan violations

3. **Scan Insertion**
   - Converted all 40 flops → **SDFF scan flops**
   - Added **SI (Scan In), SO (Scan Out), SE (Scan Enable), Reset**

4. **Scan Chain Creation**
   - Inserted **4 scan chains** (balanced: 10 flops per chain)
   - Verified connectivity

5. **Reports Generated**
   - `scan_cell.rpt` → scan cell details
   - `scan_chain.rpt` → scan chain mapping

---

## 📊 Results

- ✅ 40/40 flops converted into scan flops  
- ✅ 4 scan chains created, each of length 10  
- ✅ All clocks and resets passed stability checks  
- ✅ Netlist & scan order files successfully generated  

---

## 📂 Project Files

- `dofile/` → Tessent dofile for setup & scan insertion  
- `reports/` → DFT reports (scan cells, scan chains)  
- `outputs/` → Scan-inserted netlist and scan definition  
- `screenshots/` → Visual evidence of schematic & reports  

---

## 🖼️ Visual Snapshots

### Before (Non-scan Flop)

### After (Scan flop inserted)

### Dofile

### Scan Chain Report

### Scan Cell Report

### Terminal_log

---

## 🔮 Next Steps (Planned Roadmap)

- **Level2:** ATPG pattern generation (Stuck-at, TDF, IDDQ) + EDT compression  
- **Level3:** MBIST integration + JTAG boundary scan  

---

👤 **Author:** Asha Ranabhare  
📧 Email: asharanabhare28@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/asha-ranabhare-2ab4b824b) | [GitHub](https://github.com/asha-0905)

---
⭐ If you found this useful, consider giving the repo a **star**!
