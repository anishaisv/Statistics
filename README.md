This project performs fundamental statistical analysis on a dataset containing physiological and physical performance data. Using Python libraries like pandas, statistics, scipy, and numpy, the notebook explores key metrics like mean, median, mode, skewness, variance, harmonic mean, and quadratic mean.

🗂 Dataset Description
The dataset bodyPerformance.csv includes 12 columns and 13,393 records related to individuals' fitness and health parameters:

age: Age of the individual

gender: Gender (M/F)

height_cm: Height in centimeters

weight_kg: Weight in kilograms

body fat_%: Body fat percentage

diastolic: Diastolic blood pressure

systolic: Systolic blood pressure

gripForce: Hand grip strength

sit and bend forward_cm: Flexibility

sit-ups counts: Sit-up repetitions

broad jump_cm: Distance jumped in broad jump

class: Fitness level classification (A–D)

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

Mean: df.mean() or statistics.mean()

Median: statistics.median()

Mode: df.mode()

Variance: statistics.variance()

Distribution and Skewness

Visualized with df.plot(kind='density')

Calculated skewness with df.skew()

Advanced Metrics

Harmonic Mean: scipy.stats.hmean()

Quadratic Mean (RMS): np.sqrt(np.mean(np.square()))

📊 Sample Results
Mean Height: 168.56 cm

Median Height: 169.2 cm

Mode Height: 170 cm

Height Variance: ~71.01

Height Harmonic Mean: ~168.13

Height Quadratic Mean: ~169.0

📌 Inferences
Most individuals are aged between 25–40.

Height is slightly negatively skewed (left tail).

The dataset is clean (no missing values).

Some metrics like sit-ups counts and gripForce have a moderate skew.
