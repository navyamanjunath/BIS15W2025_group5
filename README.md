# BIS15W2025_group5


<h1 style="font-family: Arial, sans-serif;">
  <font color="#0066CC">
    BIS15L Final Project – PharmGKB Relationships
    <em>By Rithanya Siva, Navya Manjunath, Dennis Chao</em>
  </font>
</h1>

<p align="center">
  <em>A Shiny application exploring gene, variant, and disease relationships using PharmGKB data.</em>
</p>

---

## <font color="#0066CC">Overview</font>

This repository holds our final project analyzing how genes, variants, and diseases intersect in the [PharmGKB](https://www.pharmgkb.org/) `relationships.tsv` dataset. Our accompanying [presentation](https://docs.google.com/presentation/d/1NAS11obJwFwnLm5t8jDNbPjiQ8sb3igzf-h3GV3sY-s/edit#slide=id.g2582fa11c66_0_310) highlights the project’s motivation, methodology, visualizations, and results.

### <font color="#2E8B57">Key Topics</font>
1. **Introduction & Motivation**  
   - The importance of pharmacogenomics and how PharmGKB connects genes, variants, and diseases.  
   - Why **ABCB1** and **rs1045642** are central to our analysis.

2. **Data Wrangling & Cleaning**  
   - Filtering and tidying the `relationships.tsv` file using `janitor` and `dplyr`.  
   - Removing unneeded columns (PK, PD) for clearer results.

3. **ABCB1 & Variant Analysis**  
   - Identifying **ABCB1** as a frequently mentioned gene.  
   - Demonstrating **rs1045642** as a highly associated variant.

4. **Cancer Focus**  
   - Drilling down on cancer‐related diseases.  
   - Comparing clinical vs. variant evidence in bar/pie charts.

5. **Network Visualization**  
   - An interactive **visNetwork** for **ABCB1** or **rs1045642**, showing disease connections with wrapped labels.

6. **Conclusions**  
   - Key insights from our findings.  
   - Future improvements, like analyzing additional genes or refining filtering logic.

---

## <font color="#0066CC">Project Contents</font>

1. **BIS15L_Final_Project.Rmd**  
   - The main R Markdown analysis with categorization, bar/pie charts, data cleaning steps.  
2. **`app.R`** (if separate)  
   - A dedicated Shiny app script combining all data and plots into one dashboard.  
3. **`data/relationships.tsv`**  
   - The PharmGKB dataset containing entities (genes, variants, diseases, etc.). 
---

## <font color="#2E8B57">How to Run the Shiny App</font>

1. **Clone or Download** this repository to your local machine.  
2. Place **`relationships.tsv`** in the `data/` folder (or update the path in the R code). 
3. Make sure you run the entire code (all previous code chunks before the shinyapp for update datasets)
4. Open **RStudio** and set your working directory to this project.  
5. Run the Shiny app:
   - **Option A**: Knit/Run `BIS15L_Final_Project.Rmd` in RStudio.  
   - **Option B**: If an **`app.R`** file exists, do:
     ```r
     shiny::runApp("app.R")
     ```
6. A browser window will display a dashboard with these tabs:
   - **PharmGKB Analysis**  
   - **Summary Stats**  
   - **Cancer Analysis**  
   - **Network Graph**

---

## <font color="#0066CC">Summary Stats</font>

In the **Summary Stats** tab, you’ll see:
- **Total Rows** in `relationships.tsv`  
- **Unique Genes** (entity1)  
- **Unique Variants** (entity1)  
- **Unique Diseases** (entity2)  

This quick snapshot contextualizes the dataset’s scope before deeper exploration.

---

## <font color="#2E8B57">Data Usage</font>

- Downloaded from [PharmGKB](https://www.pharmgkb.org/downloads)
- PharmGKB data usage may be subject to [PharmGKB’s Terms of Use](https://www.pharmgkb.org/page/termsOfUse).

---

## <font color="#0066CC">Contact & Feedback</font>

For suggestions or questions:
- **GitHub**: [rithanyas13](https://github.com/rithanyas13), [dchao3647](https://github.com/dchao3647), [navyamanjunath](https://github.com/navyamanjunath)
- **Email**: [Rithanya Siva](mailto:rsivasubramanian@ucdavis.edu), [Dennis Chao](mailto:dcchao@ucdavis.edu), [Navya Manjunath](mailto:namanjunath@ucdavis.edu)
