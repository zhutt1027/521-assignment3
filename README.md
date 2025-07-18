# 521-assignment3： AI Dashboard Visualization

This project presents an interactive dashboard that explores global investment distribution, datapoints used in training AI, and market share of AI in different stages. It uses `Plotly` for visualizations and `Panel` for layout and interactivity.

## Visualization Technique 

The dashboard includes **four main visualizations** displayed on a single screen:

1. **Grouped Bar Chart**  
   _Annual Global AI Investment by Type_  
   ➤ Shows year-by-year investments by type (e.g., Corporate, Government).  
   ➤ Controlled by the interactive **year range slider**.

2. **Line Chart**  
   _Private AI Investment by Region_  
   ➤ Displays how private investment varies across regions over time.  
   ➤ Also controlled by the same **year slider**.

3. **Scatter Plot**  
   _Training Dataset Size over Time by Domain_  
   ➤ Illustrates datapoint growth in major AI domains (e.g., Language, Vision).  
   ➤ Controlled by a **domain selector dropdown**.  
   ➤ Uses **log-scaled y-axis** to reflect extreme data range.

4. **Pie Chart**  
   _Market Share in AI Hardware Supply Chain_  
   ➤ Visualizes stage-wise country contributions in Design, Fabrication, and Assembly.  
   ➤ Controlled by a **stage selector dropdown**.

## Visualization Libraries 

| Library  | Purpose |
|----------|---------|
| **Plotly** | Interactive visualizations (bar, pie, scatter, line) |
| **Panel** | Layouts and widgets (sliders, dropdowns, dashboard structure) |
| **Pandas** | Data handling |
| **NumPy** | Numerical operations |

##  Project Files

- `assignment3.ipynb` – Main dashboard source code  
- `ai_investment_by_region.csv`  
- `ai_investment_by_type.csv`  
- `ai_training.csv`  
- `market_share.csv`  
- `hvplot_error.png` – Reference error screenshot  
- `README.md`, `LICENSE`, `.gitignore`

## Demo Video

Watch a short demo showing all visualizations and interactivity:  
(https://drive.google.com/file/d/1u49xik1zg2iteTvTz_Ct8KDrUiiK-wq0/view?usp=sharing)

## Known Limitations

- Plotly and Panel are not fully integrated, requiring `@pn.depends` to manually link widgets and plots.  

## License

Licensed under the [Apache 2.0 License](LICENSE).
