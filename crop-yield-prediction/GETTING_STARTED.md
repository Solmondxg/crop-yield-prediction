# Getting Started Guide

## Quick Setup (3 Steps)

### 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 2️⃣ Add Your Data
- Download a crop yield dataset (see `data/README.md`)
- Place it in the `data/` folder
- Update the filename in the notebook if needed

### 3️⃣ Run the Project

**Option A: Interactive Notebook (For Learning)**
```bash
cd notebooks
jupyter notebook Uganda_Crop_Yield_Prediction.ipynb
```

**Option B: Streamlit App (For Predictions)**
```bash
streamlit run app/app.py
```

---

## Project Timeline

### Phase 1: Exploration ✅
- Load and explore data
- Analyze patterns and relationships
- Identify missing values

### Phase 2: Preparation ✅
- Clean data
- Encode categorical variables
- Split into train/test sets

### Phase 3: Modeling ✅
- Build Linear Regression model
- Build Random Forest model
- Compare performance

### Phase 4: Deployment
- [x] Save trained model
- [x] Create web app with Streamlit
- [ ] Deploy to Streamlit Cloud
- [ ] Add to portfolio website

---

## File Descriptions

| File | Purpose |
|------|---------|
| `Uganda_Crop_Yield_Prediction.ipynb` | Main notebook with complete workflow |
| `app/app.py` | Interactive web application |
| `models/` | Trained model files (pickle format) |
| `data/` | Your datasets go here |
| `requirements.txt` | Python package dependencies |
| `README.md` | Full project documentation |

---

## Common Issues & Solutions

### Issue: "Module not found" error
**Solution**: Make sure all packages in `requirements.txt` are installed:
```bash
pip install -r requirements.txt
```

### Issue: "Dataset not found"
**Solution**: 
1. Download a CSV file from Kaggle or FAO
2. Place it in the `data/` folder
3. Update the filename in the notebook

### Issue: Streamlit app won't start
**Solution**:
1. Make sure you're in the correct directory
2. Check that app.py exists in the `app/` folder
3. Try: `streamlit run app/app.py --logger.level=debug`

### Issue: Model predictions seem wrong
**Solution**:
1. Check that your data has similar format to training data
2. Verify that scale of features is reasonable
3. Review the feature importance graphs

---

## Next Steps

1. **Explore the Notebook**
   - Run each cell and understand what it does
   - Look at the visualizations
   - Try changing parameters

2. **Customize for Your Data**
   - Update column names if different
   - Adjust feature selection
   - Modify hyperparameters

3. **Deploy Online**
   - Push to GitHub
   - Connect to Streamlit Cloud
   - Share the live link

4. **Add to Portfolio**
   - Update README with your results
   - Document your approach
   - Create project description

---

## Resources

- 📖 Full Documentation: See `README.md`
- 📓 Data Guide: See `data/README.md`
- 🎥 Video Tutorials: Search "Machine Learning Project Python"
- 🔗 Kaggle Datasets: https://www.kaggle.com

---

Good luck! 🌾 Happy learning! 📊
