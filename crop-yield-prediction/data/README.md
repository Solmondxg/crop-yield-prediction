# Data Folder - README

## How to Add Your Dataset

### Step 1: Download a Dataset

Find crop yield data from one of these sources:

1. **Kaggle** (https://www.kaggle.com/)
   - Search for: "crop yield prediction", "maize yield", "agriculture Uganda"
   - Look for datasets with climate and yield information

2. **FAO** (https://www.fao.org/)
   - Search for Uganda crop statistics and agro-climatic data
   - Download historical yield records

3. **UCI Machine Learning Repository**
   - Search for crop yield or agriculture datasets

### Step 2: Prepare Your Dataset

Ensure your CSV file has these columns (or similar):
- **Year**: Year of observation (2015-2025)
- **District**: Region name (e.g., Kampala, Arua, Kigezi)
- **Rainfall_mm**: Annual rainfall in millimeters
- **Temperature_C**: Average temperature in Celsius
- **Soil_Type**: Type of soil (Sandy, Loam, Clay)
- **Season**: Growing season (Wet or Dry)
- **Fertilizer_kg_ha**: Fertilizer application rate
- **Yield_tons_ha**: Crop yield in tons per hectare (** TARGET VARIABLE **)

### Step 3: Place the File

1. Save your CSV file in this folder
2. Update the filename in the notebook if different from `uganda_maize_yield.csv`
3. Run the notebook cells to load and analyze the data

### Step 4: Folder Structure

After adding data:
```
data/
├── README.md (this file)
├── raw/
│   └── uganda_maize_yield.csv   (your original data)
└── processed/
    └── (cleaned data goes here after processing)
```

## Example CSV Format

| Year | District | Rainfall_mm | Temperature_C | Soil_Type | Season | Fertilizer_kg_ha | Yield_tons_ha |
|------|----------|-------------|---------------|-----------| -------|------------------|---------------|
| 2020 | Kampala  | 1200        | 24.5          | Loam      | Wet    | 50               | 3.5           |
| 2020 | Arua     | 1500        | 23.0          | Clay      | Wet    | 75               | 4.0           |
| 2021 | Kigezi   | 900         | 25.5          | Sandy     | Dry    | 30               | 2.5           |

## Tips for Good Data

✅ **What makes good data:**
- At least 100+ records (more is better)
- Complete data (few missing values)
- Multiple years and regions
- Realistic yield values (typically 1.5-5.5 tons/ha for maize)

❌ **Avoid:**
- Data with too many missing values
- Incomplete columns
- Only one region or year
- Extreme outliers

## Using Sample Data

If you want to start without your own dataset, the notebook includes code to generate sample data for demonstration purposes. This is perfect for learning the workflow before using real data.

## Questions?

If your dataset is structured differently:
1. Update the column names in the notebook `load_dataset` section
2. Ensure all numerical columns are properly converted to numbers
3. Update categorical encoding for your specific categories

Happy analyzing! 🌾
