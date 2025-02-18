# Irish Housing ABM

## Project Overview
This project is an **Agent-Based Model (ABM)** for simulating the Irish housing market. The model generates households and houses, assigns housing contracts, and simulates housing construction over time. It aims to provide insights into housing dynamics based on real-world data.

## Features
- **Household Generation**: Creates different household types based on predefined distributions.
- **Housing Generation**: Constructs new houses annually with different sizes, quality levels, and ownership types.
- **Housing Assignment**: Matches households to houses based on availability and predefined rules.
- **Randomized Properties**: Uses statistical distributions to determine factors like household income, house quality, and sizes.

## Project Structure
```
|-- irish_housing_abm/
    |-- Household.cs
    |-- HouseholdGenerator.cs
    |-- HouseholdDataStore.cs
    |-- House.cs
    |-- HouseGenerator.cs
    |-- ConstructionCompany.cs
    |-- RNG.cs
    |-- Program.cs
    |-- README.md
```

### Key Classes
- **Household**: Represents a household with attributes like income, wealth, and family structure.
- **HouseholdGenerator**: Creates households based on statistical data.
- **HouseholdDataStore**: Stores data related to household distributions.
- **House**: Represents an individual housing unit with attributes like size, quality, and type.
- **HouseGenerator**: Constructs houses based on yearly quotas and demand.
- **ConstructionCompany**: Manages house construction and event-driven housing creation.
- **RNG**: A random number generator class for drawing values from probability distributions.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/irish_housing_abm.git
   cd irish_housing_abm
   ```
2. Open the project in **Visual Studio** or any C# IDE.
3. Build and run the project.

## Usage
- Modify the `HouseholdDataStore` class to adjust population and housing data.
- Set the annual house construction count in `ConstructionCompany.cs`.
- Run the simulation to generate and allocate households.

## Data Sources
The model is based on statistical data including:
- Household distributions (single, married, families with children, etc.)
- Housing ownership types (owned, rented, social housing)
- House size distributions and minimum area constraints

## Future Improvements
- Incorporate economic factors affecting housing prices.
- Improve household-housing matching based on affordability and preferences.
- Extend rental vs ownership decision modeling.

