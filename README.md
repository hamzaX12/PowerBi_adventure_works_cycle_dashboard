# \# 🚴 Adventure Works Cycle: Power BI Sales Dashboard

# 

# An interactive two-page Power BI dashboard analyzing sales, profit, customers and

# discounts for Adventure Works Cycle (2018-2021).

# 

# !\[Overview](images/page1\_overview.png)

# 

# 

# \## 🎯 Objectives

# \- Track overall sales, profit and orders

# \- Identify top categories, products and territories

# \- Analyze trends over time (YoY, MoM, YTD)

# \- Understand customer behavior and the impact of discounts

# 

# \## 📊 Key Insights

# \- Bikes generate \~95M of the 109.8M total sales (\~87%)

# \- The United States is the top market with 63M in sales

# \- Total profit is 12.55M across 121K orders

# \- \*(add 2-3 insights from your page 2: margin, YoY growth, top customers)\*

# 

# \## 🗂️ Dashboard Pages

# \### Page 1: Sales Overview

# Total sales / profit / orders, sales by category, territory and subcategory,

# top 10 products.

# !\[Page 1](images/page1\_overview.png)

# 

# \### Page 2: Performance \& Customer Insights

# Profit margin, YoY trends, customer analysis, channels and discount bands.

# !\[Page 2](images/page2\_performance.png)

# 

# \## 🧱 Data Model

# Star schema with `Sales` as the fact table and the dimensions `Product`, `Date`,

# `Customer`, `Reseller`, `SalesOrder` and `SalesTerritory`.

# !\[Model](images/data\_model.png)

# 

# \## 🧮 DAX Highlights

# ```DAX

# Profit Margin % = DIVIDE(\[Total Profit], \[Total Sales])

# Sales YoY % = DIVIDE(\[Total Sales] - \[Sales LY], \[Sales LY])

# Sales YTD = TOTALYTD(\[Total Sales], 'Date'\[Date], "6/30")

# ```

# Full list in \[`dax/measures.dax`](dax/measures.dax).

# 

# \## 🛠️ Tools

# Power BI Desktop · DAX · Power Query · Data modeling (star schema)

# 

# \## 📁 Repository Structure

# | Folder | Content |

# |---|---|

# | `dashboard/` | Power BI file (.pbix) |

# | `report/` | PDF export of the report |

# | `data/` | Source dataset |

# | `dax/` | DAX measures |

# | `images/` | Screenshots |

# 

# \## ▶️ How to Use

# 1\. Clone the repo: `git clone https://github.com/hamzaX12/PowerBi\_adventure\_works\_cycle\_dashboard.git`

# 2\. Open `dashboard/AdventureWorks\_Dashboard.pbix` in Power BI Desktop

# 3\. If prompted, point the data source to the `data/` folder

# 

# \## 👤 Author

# \*\*Hamza\*\*: \[LinkedIn](https://www.linkedin.com/in/hamza-ben-allou-48ab31236) · \[GitHub](https://github.com/hamzaX12)

