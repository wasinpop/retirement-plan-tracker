# Retirement Plan Tracker

A comprehensive, single-page web application designed to help users plan for their retirement. This tool provides detailed projections, visualizations, and analysis tools to give a clear picture of one's financial journey towards retirement.

## ✨ Features

* **Comprehensive Inputs:** Model your financial future with inputs for current age, retirement age, life expectancy, assets, savings, spending goals, and expected returns.
* **Dynamic Projections:** Instantly see the impact of your inputs on your retirement plan.
* **Interactive Chart:** Visualize your lifetime wealth projection with an interactive line chart showing your balance over time.
* **Detailed Data Tables:** View year-by-year, month-by-month, and drawdown projections in easy-to-read tables.
* **Goal Seeking Analysis:**
    * **Find Required Savings:** Automatically calculate the monthly savings needed to reach your retirement goal.
    * **Find Earliest Retirement Age:** Determine the earliest age you can retire based on your current plan.
* **Stress Testing:**
    * **Lower Return Scenario:** See how your plan holds up with a lower pre-retirement investment return.
    * **Longevity Scenario:** Calculate the nest egg required to fund a longer life expectancy (until age 95).
* **Light & Dark Modes:** A sleek, modern interface with a theme toggle for user comfort.
* **Persistent State:** Your input values are saved in your browser's local storage, so your data is preserved between sessions.
* **Fully Responsive:** The layout is optimized for desktops, tablets, and mobile devices.

## 🚀 How to Use

1.  **Open the Tool:** Simply open the `index.html` file in any modern web browser.
2.  **Enter Your Data:** Fill in the fields in the "Your Profile & Goals" section. All calculations update in real-time as you type.
3.  **Analyze the Outlook:**
    * The **Retirement Outlook** card shows your target nest egg, your projected savings, and the resulting surplus or shortfall.
    * The **Lifetime Wealth Projection** chart visualizes your financial growth and drawdown.
    * The **Stress Tests** card provides insight into potential risks.
4.  **Explore Projections:** Use the tabs (Yearly, Monthly, Drawdown) to see the detailed breakdown of your financial journey.
5.  **Use Analysis Tools:** Click the "Find Required Savings" or "Find Earliest Retirement Age" buttons to solve for key variables in your plan.

## 🛠️ Technologies Used

* **HTML5:** For the core structure and content.
* **Tailwind CSS:** For a utility-first, responsive, and modern design.
* **JavaScript (ES6+):** For all the calculation logic, DOM manipulation, and interactivity.
* **Chart.js:** For creating the beautiful and interactive projection chart.
* **chartjs-plugin-annotation:** To add the vertical retirement line to the chart.

## 🧮 Core Calculations

* **Accumulation Phase:** A compound interest formula is applied monthly, factoring in monthly contributions and an annual increase in those contributions.
* **Drawdown Phase:** A present value of an annuity formula is used to calculate the required nest egg (Retirement Goal). This calculation accounts for post-retirement returns and inflation to determine how much is needed to fund the desired annual spending.
* **Goal Seeking:** The analysis tools use iterative algorithms (binary search for savings, linear search for age) to find the input values that satisfy the retirement goal.

## 📄 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
