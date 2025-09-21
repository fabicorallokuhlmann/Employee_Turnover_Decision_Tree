  <h1>📊 Employee Turnover Decision Tree</h1>

  <p>
  The main purpose of this study is to understand the relationship between employee survey scores (leadership, communication, engagement, etc.) and voluntary turnover, specifically    focusing on cases where employees reported leaving for “more attractive opportunities” while still within the defined salary range.
  </p>

  <hr>

  <h2>🧠 Objectives</h2>
  <ul>
    <li>Merge survey and turnover data by business unit.</li>
    <li>Explore correlations between topics and turnover.</li>
    <li>Build models to identify key turnover drivers.</li>
    <li>Key steps in the analysis include:</li>
      <ul>
       <ul>
        <li>Load and merge turnover and survey datasets</li>
        <li>Correlation analysis and visualization</li>
        <li>Regression analysis and R² evaluation</li>
        <li>ANOVA testing</li>
        <li>Decision tree modeling and feature importance</li>
        <li>Multiple linear regression</li>
</ul>
</section>
      </ul>
    </li>
  </ul>

  <hr>

  <h2>📁 Dataset</h2>
  <ul>
    <li><strong>desligamentos.xlsx</strong>: turnover metrics per business unit.</li>
    <li><strong>Pasta3.xlsx</strong>: employee satisfaction survey scores.</li>
  </ul>
  <p>Both datasets are merged using the <code>Franquia</code> column.</p>

  <hr>

  <h2>🛠️ Requirements</h2>
  <pre><code>pip install pandas seaborn matplotlib scikit-learn statsmodels scipy</code></pre>

  <hr>

  <h2>🔍 Code Overview</h2>

  <h3>1. Load Data</h3>
  <p>Reads both Excel files into DataFrames using <code>pandas</code>.</p>

  <h3>2. Merge by Unit</h3>
  <p>Combines datasets by the <code>Franquia</code> column to unify analysis.</p>

  <h3>3. Correlation Matrix</h3>
  <p>Calculates and visualizes Pearson correlations between all numeric variables.</p>

  <h3>4. Heatmap</h3>
  <p>Shows how each survey topic correlates with voluntary, involuntary, and general turnover.</p>

  <h3>5. Regression Plots</h3>
  <p>Performs simple linear regressions between each survey score and a selected turnover metric. R² values are shown on the plots.</p>

  <h3>6. ANOVA</h3>
  <p>Example using <strong>Compensation</strong> score to check if differences in score significantly affect turnover.</p>

  <h3>7. Decision Tree</h3>
  <p>Fits a regression tree to discover score combinations that best predict turnover. Visualizes tree and stores the leaf node for each sample.</p>

  <h3>8. Multiple Linear Regression</h3>
  <p>Builds a full model with all scores as predictors of turnover. Outputs full statistical summary.</p>

  <h3>9. Feature Importance</h3>
  <p>Extracts and plots the importance of each score from the decision tree model.</p>

  <h3>🔁 Optional: Rule-Based Segmentation</h3>
  <p>Commented-out logic allows custom group creation based on score thresholds and tree splits.</p>

  <hr>
  

  <h2>📈 Outputs</h2>
  <ul>
    <li>Correlation heatmap</li>
    <li>R² regression plots</li>
    <li>ANOVA table</li>
    <li>Decision tree visualization</li>
    <li>Multiple regression summary</li>
    <li>Feature importance barplot</li>
  </ul>

  <hr>

  <h2>📌 Notes</h2>
  <ul>
    <li>You can change the analyzed turnover type by modifying this line:</li>
  </ul>
  <pre><code>tipo_desligamento = '%Desligamento (voluntário)'</code></pre>
  <ul>
    <li>Ensure the column names match your Excel file exactly.</li>
    <li>Replace hardcoded file paths with relative paths or file input if needed.</li>
  </ul>

  <hr>

  <h2>👩‍💻 Author</h2>
  <p><strong>Fabiana Corallo Mello de Azevedo Kuhlmann</strong></p>

  <hr>

  <h2>📄 License</h2>
  <p>This project is licensed under the MIT License. You are free to use, modify, and distribute it with proper attribution.</p>

</body>
</html>


