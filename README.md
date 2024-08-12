# DIY Covid-19 Dashboard

Welcome to the DIY Covid-19 Dashboard repository! This project provides an interactive dashboard to visualize and compare Covid-19 data for England and Scotland. The dashboard is built using Python, leveraging various data visualization and interactive libraries.

## Features

- **Interactive Data Visualization**: The dashboard allows users to select and visualize Covid-19 cases, hospitalizations, and deaths for England and Scotland.
- **Real-Time Data Updates**: Users can refresh the dashboard to fetch the latest Covid-19 data from the Public Health England (PHE) API and visualize it instantly.
- **Customizable Graphs**: The dashboard provides options to select specific data categories (cases, hospitalizations, deaths) and to choose between linear or logarithmic scales for graph visualization.

## Getting Started

### Prerequisites

Ensure you have the following Python packages installed:

```bash
pip install ipywidgets pandas numpy matplotlib uk-covid19
```

### Running the Dashboard

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/diy-covid-dashboard.git
   cd diy-covid-dashboard
   ```

2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

3. Open the `covid_dashboard.ipynb` notebook and run all cells to start the dashboard.

### Dashboard Overview

#### England Dashboard

The dashboard for England allows users to:

- **Select Data**: Use the "Stats" widget to select one or more categories (cases, hospitalizations, deaths) to visualize.
- **Choose Scale**: Select between a linear or logarithmic scale for the y-axis of the graph.
- **Refresh Data**: Click the "Refresh Data" button to retrieve the latest data from the PHE API.

#### Scotland Dashboard

Similarly, the Scotland dashboard provides:

- **Select Data**: Choose from cases, hospitalizations, and deaths for visualization.
- **Choose Scale**: Switch between linear and logarithmic scales.
- **Refresh Data**: Update the graph with the most recent data by pressing the "Refresh Data" button.

## Code Structure

- **Data Wrangling**: The `wrangle_data()` function processes raw Covid-19 data into a time series format suitable for plotting.
- **API Access**: The `access_api()` and `access_api_scotland()` functions fetch the latest Covid-19 data for England and Scotland, respectively.
- **Graph Refreshing**: The `refresh_graph()` and `refresh_graph_scotland()` functions update the graphs based on user-selected options.
- **Interactive Controls**: Widgets (dropdowns, radio buttons) enable users to customize the data displayed on the graphs.

## Contributing

Contributions are welcome! If you find a bug or have a feature request, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Data provided by [Public Health England (PHE)](https://www.gov.uk/government/organisations/public-health-england) and the [uk-covid19](https://pypi.org/project/uk-covid19/) Python package.
- Interactive widgets powered by [ipywidgets](https://ipywidgets.readthedocs.io/).

---

