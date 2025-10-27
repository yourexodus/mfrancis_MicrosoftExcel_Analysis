# 🎧 Music Industry Revenue Project: Composition Analysis

This repository contains the analysis and visualization of music industry revenue over a 40-year period, focusing on the shift in composition between **Physical** and **Digital** formats.

---

## 🎯 Project Goal

The primary objective was to visualize the **revenue composition over time** for Physical and Digital music products to communicate the industry's historical transition to a general audience.

---

## 📂 Source Data and Context

| Detail | Description |
| :--- | :--- |
| **Data Type** | Time Series |
| **Format** | Excel Spreadsheet |
| **Key Insight** | Revenue figures are in **Millions**, requiring specific axis formatting. |
| **Communication Goal** | Composition over time (40 years) |
| **Target Audience** | General Public |
| **Visualization Choice** | **Stacked Area Chart** |

### Initial Assets

* **Original Request/Context:**
    * `[Image: email_context.png]`
* **Source Data Screenshot:**
    * `[Image: raw_data_screenshot.png]`

---

## 📈 Visualization Development Steps

The following steps detail the creation and formatting of the final **Stacked Area Chart** using data visualization best practices.

### 1. Chart Selection and Data Order

1.  **Selection:** Inserted a standard Stacked Area Chart after selecting the entire data range.
2.  **Fixing Stacking Order:** The initial chart obscured the Digital baseline. This was corrected by switching the series order so that **Digital** appeared *first* in the data list, allowing its baseline to be visible.

### 2. Formatting for Clarity (Reducing Noise)

| Action | Technique | Before | After |
| :--- | :--- | :--- | :--- |
| **Add Title** | Clearly labeled the chart to inform the user. | `[Image: chart_before_title.png]` | `[Image: chart_after_title.png]` |
| **Remove Border** | Set **Shape Outline** to **No Outline**. | `[Image: chart_before_border.png]` | `[Image: chart_after_border.png]` |
| **Remove Gridlines** | Unchecked the **Gridlines** option (or manually deleted them). | `[Image: chart_before_grid.png]` | `[Image: chart_after_grid.png]` |

### 3. Cleaning Up the Y-Axis (Revenue)

A custom number format was applied to correctly display revenue in billions and reduce redundant zeros, making the axis labels scannable.

1.  **Access Formatting:** Right-click Y-Axis $\rightarrow$ **Format Axis** $\rightarrow$ **Number** $\rightarrow$ **Custom**.
2.  **Initial Adjustment (Millions):** Added `"M"` to the end of the format string (e.g., `\$#,##0"M"`).
3.  **Final Adjustment (Billions):** Changed the format to tell Excel to drop the last three digits and display the scale in Billions.
    * **Final Custom Format:** `\$#,##0, "B"` (The comma before "B" scales the number by $1,000$).
4.  **Axis Title:** Added the title **Revenue** to the primary vertical axis.

### 4. Final Polish and Legend Removal

1.  **Set Text Size:** Standardized all axis labels to **Text Size 11**.
2.  **Direct Labeling:** Instead of using the legend, text boxes were added directly to the chart areas for **PHYSICAL** and **DIGITAL** (improving data ink ratio).
    * The redundant chart legend was then **deleted**.

---

## ✨ Final Visualization

The completed chart provides a clean, highly formatted visualization of the music industry's composition shift.

`[Image: final_chart.png]`

---

Feel free to replace the placeholder image tags with actual links or file paths once you upload your images to the repository! Would you like any of these sections expanded or linked to a separate document (like a `ANALYSIS.md`)?