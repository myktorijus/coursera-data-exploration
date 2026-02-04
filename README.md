<h1>Coursera Dataset Exploration</h1>
<p>
  This repository contains a Jupyter Notebook project where I explore a Coursera Course Dataset from Kaggle using
  <strong>pandas</strong> for EDA and data cleaning, and <strong>matplotlib/seaborn</strong> for visualization.
  The goal is to understand the dataset composition and spot patterns related to course popularity (enrollment) and course quality signals (ratings).
</p>

<h2>Project Overview</h2>
<ul>
  <li><strong>Data source:</strong> Coursera Course Dataset (Kaggle)</li>
  <li><strong>Key focus:</strong> basic EDA, cleaning, dtype optimization, and clear visual storytelling</li>
  <li><strong>Outputs:</strong> a cleaned dataset export + an analysis notebook with charts and conclusions</li>
</ul>

<h2>Repository Structure</h2>
<ul>
  <li><strong>assets/</strong> — images used in the notebook header</li>
  <li><strong>data/</strong> — raw and cleaned CSV files</li>
  <li><strong>notebook/</strong> — the main Jupyter Notebook (<code>.ipynb</code>)</li>
  <li><strong>requirements.txt</strong> — project dependencies</li>
  <li><strong>435.md</strong> — description of the sprint assignment</li>
  <li><strong>.gitignore</strong> — ignored files/folders</li>
  <li><strong>README.md</strong> — project overview (how to run, what’s inside, repo structure)</li>
</ul>

<h2>Dataset Columns</h2>
<ul>
  <li><code>course_title</code> — course title</li>
  <li><code>course_organization</code> — course provider (university/company)</li>
  <li><code>course_Certificate_type</code> — certificate format (Course / Specialization / Professional Certificate)</li>
  <li><code>course_rating</code> — course rating</li>
  <li><code>course_difficulty</code> — difficulty level</li>
  <li><code>course_students_enrolled</code> — enrollment (stored in abbreviated text form in the raw dataset)</li>
</ul>

<h2>What’s Inside the Notebook</h2>
<ul>
  <li><strong>Data loading & inspection</strong>: shape, dtypes, unique values, duplicate checks</li>
  <li><strong>Cleaning & validation</strong>:
    <ul>
      <li>dtype optimization (string/category/float32/int32) to reduce memory usage</li>
      <li>parsing enrollment values (e.g., <code>5.3k</code>, <code>3.2m</code>) into a numeric column</li>
      <li>basic text cleanup (whitespace normalization)</li>
      <li>sanity checks for numeric ranges</li>
    </ul>
  </li>
  <li><strong>EDA questions</strong> (answered with visualizations):
    <ul>
      <li>Distribution of certificate types</li>
      <li>Enrollment by certificate type</li>
      <li>Distribution of difficulty levels</li>
      <li>Top organizations by number of courses</li>
      <li>Top organizations by total enrollment</li>
      <li>Top organizations by enrollment per course (with a minimum-course threshold)</li>
      <li>Ratings by difficulty</li>
      <li>Relationship between rating and enrollment</li>
    </ul>
  </li>
  <li><strong>Key insights & suggested improvements</strong>: concise findings + limitations and next steps</li>
</ul>

<h2>How to Run</h2>
<ol>
  <li>Install Python 3.10+ (recommended)</li>
  <li>Create and activate a virtual environment</li>
  <li>Install dependencies:
    <pre><code>pip install -r requirements.txt</code></pre>
  </li>
  <li>Open and run the notebook:
    <ul>
      <li>in VS Code: open the <code>.ipynb</code> inside <code>notebook/</code> and select the project kernel</li>
      <li>or with Jupyter:
        <pre><code>jupyter notebook</code></pre>
      </li>
    </ul>
  </li>
</ol>

<h2>Notes</h2>
<ul>
  <li>The cleaned dataset is exported to the <code>data/</code> folder for reuse.</li>
  <li>Some comparisons are limited by small group sizes (e.g., Professional Certificates, Advanced difficulty), and the notebook explicitly calls this out.</li>
  <li>This is an EDA-focused project: the goal is insight and clarity, not predictive modeling.</li>
</ul>
