This project performs fundamental statistical analysis on a dataset containing physiological and physical performance data. Using Python libraries like pandas, statistics, scipy, and numpy, the notebook explores key metrics like mean, median, mode, skewness, variance, harmonic mean, and quadratic mean.

🗂 Dataset Description
The dataset bodyPerformance.csv includes 12 columns and 13,393 records related to individuals' fitness and health parameters:

🔧 Libraries Used
pandas — Data manipulation and analysis
statistics — Built-in Python module for basic stats
numpy — Numerical operations (especially RMS)
scipy.stats — Advanced statistics (e.g., harmonic mean)
matplotlib / pandas.plotting — For plotting density curves

📈 Steps Performed
Load and Explore the Dataset
Used pd.read_csv() to load the dataset
Verified types and structure with df.info() and df.describe()
Filter Numerical Columns
Removed categorical columns (gender, class)
Selected only numerical columns using select_dtypes()
Calculated Descriptive Statistics
Calculated Mean: df.mean() or statistics.mean()
Calculated Median: statistics.median()
Calculated Mode: df.mode()
Calculated Variance: statistics.variance()
Calculated Distribution and Skewness
Visualized with df.plot(kind='density')
Calculated skewness with df.skew()
Calculated Advanced Metrics
Harmonic Mean: scipy.stats.hmean()
Quadratic Mean (RMS): np.sqrt(np.mean(np.square()))



Height is slightly negatively skewed (left tail).

The dataset is clean (no missing values).

Some metrics like sit-ups counts and gripForce have a moderate skew.
