# AXZ Oil and Gas — Production Performance Review
### Weeks 1–4 | Four-Location Operational Analysis | Isaac Okolie | Power BI

---

## 📌 The Business Context

AXZ Oil and Gas Production Company launched operations across four rig locations
in the Niger Delta region — Brass, Ekeremor, Nembe, and Southern Ijaw. Four weeks
in, management needed answers. Production data was being collected at individual
employee level across all four rigs, but no structured analysis existed to tell
them whether they were meeting targets, which locations were underperforming, and
why the gaps existed.

This project was commissioned to investigate the four-week dataset, answer nine
specific management questions, and deliver an interactive Power BI dashboard that
gives leadership a clear operational picture — by location, by KPI, and by week.

---

## ❗ The Business Problem

Management set four performance targets at the start of operations. Without an
analytical layer on top of the weekly data, they had no way to:

- Compare all four rig locations across all four KPIs simultaneously
- Identify which locations were driving cost overruns or quality failures
- Determine whether training investment was producing measurable results
- Detect underperformance before it compounded over multiple weeks

The data existed. The questions had been asked. This analysis was built to
answer them.

---

## 🎯 Performance Targets

| Target | Metric | Threshold |
|--------|--------|-----------|
| Production | UPH — Units Per Hour | ≥ 11 units/hour |
| Cost | CPU — Cost Per Unit | ≤ ₦750 per unit |
| Quality | UPI — Units Per Issue | ≥ 250 units before a defect |
| Training | Training Hours | ≥ 1 hour per staff member per week |

---

## 📊 Dataset Overview

| Property | Detail |
|----------|--------|
| Total Records | 452 employee-week records |
| Employees | 113 unique employees |
| Time Period | 4 weeks of operation |
| Locations | Brass, Ekeremor, Nembe, Southern Ijaw |
| Source Files | week_1.xlsx, week_2.xlsx, week_3.xlsx, week_4.xlsx |
| Tool | Microsoft Power BI |

**Key Fields:** Employee ID, Rig Location, Hours Worked, Units Produced,
Quality Issues, Production Cost (₦), Training Hours

---

## 📈 Overall KPIs (4-Week Summary)

| KPI | Achieved | Target | Status |
|-----|---------|--------|--------|
| UPH | 11.02 | 11.0 | ✅ MET (+0.19%) |
| CPU | ₦898 | ₦750 | ❌ MISSED (-19.75%) |
| UPI | 232 | 250 | ❌ MISSED (-7.03%) |
| Training | 1.11 hrs/week | 1.0 hr/week | ✅ MET overall |
| Total Units | 285,124 | — | — |
| Total Cost | ₦220,395,000 | — | — |
| Total Quality Issues | 1,557 | — | — |

---

## 🏭 Performance by Location

| Location | UPH | CPU | UPI | Training | Employees |
|---------|-----|-----|-----|---------|----------|
| **Brass** | 11.20 ✅ | ₦717 ✅ | 246.7 ❌ | 1.55 hrs ✅ | 39 |
| **Ekeremor** | 10.95 ❌ | ₦1,009 ❌ | 122.2 ❌ | 0.76 hrs ❌ | 29 |
| **Nembe** | 11.15 ✅ | ₦689 ✅ | 209.8 ❌ | 1.18 hrs ✅ | 34 |
| **Southern Ijaw** | 11.03 ✅ | ₦910 ❌ | 150.1 ❌ | 0.69 hrs ❌ | 20 |

---

## 🔗 Training & Working Hours Impact (Correlation Analysis)

| Relationship | r Value | Strength | What It Means |
|-------------|---------|----------|---------------|
| Training Hrs → UPH | 0.48 | Moderate Positive | More training = higher productivity |
| Training Hrs → CPU | -0.66 | Moderate-Strong Negative | More training = lower cost per unit |
| Training Hrs → UPI | **0.79** | **Strong Positive** | **More training = far fewer quality defects** |
| Hours Worked → UPH | 0.47 | Moderate Positive | Longer hours = higher output rate |
| Hours Worked → CPU | **-0.88** | **Very Strong Negative** | **Longer hours = dramatically lower cost** |
| Hours Worked → UPI | 0.80 | Strong Positive | Longer hours = better quality |

---

## 💡 Key Insights

**1. The headline UPH metric is misleading**
Production volume is the only target being met. Cost is 19.75% over budget and
every single location is failing the quality standard. Management should not
declare operations healthy based on UPH alone.

**2. Ekeremor is the network's most critical underperformer**
The only location failing all four targets simultaneously. Its CPU of ₦1,009
represents an estimated ₦14.2M in excess costs over four weeks. Its UPI of 122
means quality failures are occurring twice as frequently as management expects.

**3. Brass proves the targets are achievable**
Meeting three of four targets with a fourth just 1.3% short — Brass demonstrates
that the performance standards are realistic. The question is not whether they
can be met. It is what the other locations need to change.

**4. Training is the highest-leverage intervention available**
A correlation of 0.79 between training hours and UPI is the strongest signal in
the data. The two locations missing the training target (Ekeremor, Southern Ijaw)
are the same two locations with the worst quality performance. This alignment
cannot be dismissed as coincidence.

**5. Working hours drive cost efficiency more powerfully than any other variable**
The -0.88 correlation between hours worked and CPU is the strongest relationship
in the entire dataset. The high cost-per-unit at Ekeremor and Southern Ijaw
directly mirrors their lower average working hours.

---

## ✅ Business Recommendations

| Recommendation | Expected Impact |
|---------------|----------------|
| Enforce 1-hr training minimum at Ekeremor & S.Ijaw | UPI improvement within 2–4 weeks based on 0.79 correlation |
| Commission cost audit at Ekeremor | Identify root cause of ₦1,009 CPU and recover ₦14M+ in overspend |
| Replicate Brass operational model across locations | Evidence-based performance framework from proven internal practices |
| Review Southern Ijaw workforce sizing | CPU reduction toward ₦750 through scale or consolidation |
| Weekly location-level performance reviews | Detect underperformance in days rather than weeks |

---

## 🖥️ Dashboard Features

**4-page interactive Power BI dashboard:**

| Page | Focus | Key Visuals |
|------|-------|------------|
| Page 0 | Operational Overview | KPI cards, location bar charts, employee & training charts |
| Page 1 | Training Hours Impact | Gauge charts (r values) + scatter plots for UPH, CPU, UPI |
| Page 2 | Hours Worked Impact | Gauge charts + scatter plots — reveals -0.88 CPU correlation |
| Page 3 | Rig-Level Detail | Full data table with variance % by individual rig |

**Interactive filter:** Hour-range buttons (20–40, 41–60, 61–80, 81–100 hrs)
allow analysis to be segmented by working hours band across all pages.

---

## 🏆 Skills Demonstrated

| Skill | Application |
|-------|------------|
| Power Query (M Language) | Combined 4 weekly files, added Week dimension, validated 452 records |
| DAX Measures | Dynamic UPH, CPU, UPI calculations; targets; variances; Pearson correlation |
| Power BI Dashboard Design | 4-page interactive dashboard with filters and conditional formatting |
| Correlation Analysis | Quantified training and hours relationships with all three KPIs |
| Business Translation | Converted data patterns into cost estimates and actionable recommendations |

---

## ⚠️ Limitations

- 4 weeks is a short observation period — patterns may shift as operations mature
- Correlation does not prove causation — further investigation is needed
- No external factors (equipment age, materials, environment) are captured
- No financial P&L data to translate cost overruns into margin impact

---

## 🔮 Future Improvements

- Extend dataset to 8–12 weeks for trend analysis
- Build predictive model using training/hours to forecast KPI outcomes
- Add individual employee performance page for peer coaching identification
- Integrate revenue and margin data for profitability view
- Automate weekly KPI alerts for real-time management notification

---

## 📁 Project Structure

```
AXZ-OilRig-Performance/
│
├── README.md
├── AXZ_OilRig_Performance_Report.pdf
├── week_1.xlsx
├── week_2.xlsx
├── week_3.xlsx
├── week_4.xlsx
├── Oil_Rig_Project_Business_Brief.pdf
└── screenshots/
    ├── dashboard_overview.png
    ├── dashboard_training_correlation.png
    ├── dashboard_hours_correlation.png
    └── dashboard_detail_table.png
```

---

## 👤 About Me

**Isaac Okolie**
Data Analyst & Data Analytics Tutor | Nigeria

I specialize in transforming raw operational data into actionable business
intelligence. This project demonstrates end-to-end analytics — from multi-file
data combination and KPI modeling to correlation analysis and executive dashboard
design — all grounded in a real business brief with specific management questions.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/in/isaac-okolie)

---

*AXZ Oil and Gas Production Company | SkillAhead Analytics | Power BI | Weeks 1–4*
