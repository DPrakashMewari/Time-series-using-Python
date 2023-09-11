<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="Time_Series_0"></a>Time Series</h1>
<p class="has-line-data" data-line-start="2" data-line-end="3">A time series is a sequence of data points collected over time, often used for analysis, forecasting, and understanding trends.</p>
<p class="has-line-data" data-line-start="4" data-line-end="5">In time series, we often perform extrapolation to find values outside the observed range.</p>
<h2 class="code-line" data-line-start=6 data-line-end=7 ><a id="Time_Series_Components_6"></a>Time Series Components</h2>
<ol>
<li class="has-line-data" data-line-start="8" data-line-end="9"><strong>Trend</strong></li>
<li class="has-line-data" data-line-start="9" data-line-end="10"><strong>Seasonality</strong></li>
<li class="has-line-data" data-line-start="10" data-line-end="11"><strong>Cyclic</strong></li>
<li class="has-line-data" data-line-start="11" data-line-end="13"><strong>Noise</strong></li>
</ol>
<h3 class="code-line" data-line-start=13 data-line-end=14 ><a id="Data_Preprocessing_Required_13"></a>Data Preprocessing (Required)</h3>
<ul>
<li class="has-line-data" data-line-start="15" data-line-end="16"><strong>Handling Missing Values</strong></li>
<li class="has-line-data" data-line-start="16" data-line-end="17"><strong>Handling Outliers</strong></li>
<li class="has-line-data" data-line-start="17" data-line-end="19"><strong>Handling Time Zones</strong></li>
</ul>
<h3 class="code-line" data-line-start=19 data-line-end=20 ><a id="Exploratory_Data_Analysis_19"></a>Exploratory Data Analysis</h3>
<ul>
<li class="has-line-data" data-line-start="21" data-line-end="22"><strong>Linear Chart</strong></li>
<li class="has-line-data" data-line-start="22" data-line-end="23"><strong>Area Chart</strong></li>
<li class="has-line-data" data-line-start="23" data-line-end="24"><strong>Seasonal Check</strong></li>
<li class="has-line-data" data-line-start="24" data-line-end="25"><strong>Outlier Analysis</strong></li>
<li class="has-line-data" data-line-start="25" data-line-end="26"><strong>Lag Plot</strong></li>
<li class="has-line-data" data-line-start="26" data-line-end="28"><strong>Rolling Statistics</strong></li>
</ul>
<h3 class="code-line" data-line-start=28 data-line-end=29 ><a id="Stationary_Check_28"></a>Stationary Check</h3>
<ul>
<li class="has-line-data" data-line-start="30" data-line-end="31"><strong>Visual Inspection</strong></li>
<li class="has-line-data" data-line-start="31" data-line-end="32"><strong>Summary Statistics</strong>: If mean and variance are not constant, it’s not stationary</li>
<li class="has-line-data" data-line-start="32" data-line-end="34"><strong>ADF Test (Augmented Dickey-Fuller Test)</strong></li>
</ul>
<p class="has-line-data" data-line-start="34" data-line-end="35">If the data is not stationary, we perform data transformation.</p>
<h3 class="code-line" data-line-start=36 data-line-end=37 ><a id="Data_Transformation_36"></a>Data Transformation</h3>
<ul>
<li class="has-line-data" data-line-start="38" data-line-end="39"><strong>Differencing</strong></li>
<li class="has-line-data" data-line-start="39" data-line-end="40"><strong>Log Transformation</strong></li>
<li class="has-line-data" data-line-start="40" data-line-end="42"><strong>Box-Cox Transform</strong></li>
</ul>
<p class="has-line-data" data-line-start="42" data-line-end="43">Remember, it’s an iterative process.</p>
<h3 class="code-line" data-line-start=44 data-line-end=45 ><a id="Decomposition_44"></a>Decomposition</h3>
<ul>
<li class="has-line-data" data-line-start="46" data-line-end="47"><strong>Trend</strong></li>
<li class="has-line-data" data-line-start="47" data-line-end="48"><strong>Seasonality</strong></li>
<li class="has-line-data" data-line-start="48" data-line-end="50"><strong>Residual</strong></li>
</ul>
<h3 class="code-line" data-line-start=50 data-line-end=51 ><a id="ACF_and_PACF_AutoCorrelation_Function_and_Partial_AutoCorrelation_Function_50"></a>ACF and PACF (AutoCorrelation Function and Partial AutoCorrelation Function)</h3>
<p class="has-line-data" data-line-start="52" data-line-end="53">Used to identify potential orders for all models.</p>
<ul>
<li class="has-line-data" data-line-start="54" data-line-end="55"><strong>Autocorrelation</strong>: Measures the correlation of a time series with its past values. Positive at Lag-1 suggests AR, negative suggests MA.</li>
<li class="has-line-data" data-line-start="55" data-line-end="57"><strong>Partial Autocorrelation</strong>: Measures correlation controlling for another set of variables. Quick decay suggests AR terms, slow decay suggests MA terms.</li>
</ul>
<h2 class="code-line" data-line-start=57 data-line-end=58 ><a id="Model_Selection_Different_Models_57"></a>Model Selection (Different Models)</h2>
<ol>
<li class="has-line-data" data-line-start="59" data-line-end="63">
<p class="has-line-data" data-line-start="59" data-line-end="60"><strong>Simple Moving Average</strong>: Smoothing of time series data.</p>
<ul>
<li class="has-line-data" data-line-start="60" data-line-end="61">Cumulative Moving Average</li>
<li class="has-line-data" data-line-start="61" data-line-end="63">Exponential Moving Average</li>
</ul>
</li>
<li class="has-line-data" data-line-start="63" data-line-end="65">
<p class="has-line-data" data-line-start="63" data-line-end="64"><strong>ARIMA (AutoRegressive Integrated Moving Average)</strong>: Displayed as (p, d, q), where p is periods to lag for, d is the number of transformations used to make the data stationary, q is lags of the error component.</p>
</li>
<li class="has-line-data" data-line-start="65" data-line-end="72">
<p class="has-line-data" data-line-start="65" data-line-end="66"><strong>Seasonal SARIMA (Seasonal AutoRegressive Integrated Moving Average)</strong>: Extends ARIMA to handle seasonality.</p>
<pre><code class="has-line-data" data-line-start="68" data-line-end="71" class="language-python">order = (<span class="hljs-number">1</span>, <span class="hljs-number">1</span>, <span class="hljs-number">1</span>)  <span class="hljs-comment"># Non-seasonal order (p, d, q)</span>
seasonal_order = (<span class="hljs-number">1</span>, <span class="hljs-number">1</span>, <span class="hljs-number">1</span>, <span class="hljs-number">7</span>)  <span class="hljs-comment"># Seasonal order (P, D, Q, S)</span>
</code></pre>
</li>
<li class="has-line-data" data-line-start="72" data-line-end="78">
<p class="has-line-data" data-line-start="72" data-line-end="73"><strong>Vector AutoRegressive (VAR)</strong>: Considers the relationship between multiple time series variables.</p>
<pre><code class="has-line-data" data-line-start="75" data-line-end="77" class="language-python">model = VAR(df[[<span class="hljs-string">'data1'</span>, <span class="hljs-string">'data2'</span>]])
</code></pre>
</li>
</ol>
<h2 class="code-line" data-line-start=78 data-line-end=79 ><a id="Model_Training_and_Testing_78"></a>Model Training and Testing</h2>
<ul>
<li class="has-line-data" data-line-start="80" data-line-end="81">Split data into train and test sets.</li>
<li class="has-line-data" data-line-start="81" data-line-end="83">Use the selected model to predict for the test data.</li>
</ul>
<h2 class="code-line" data-line-start=83 data-line-end=84 ><a id="Model_Evaluation_83"></a>Model Evaluation</h2>
<ul>
<li class="has-line-data" data-line-start="85" data-line-end="86"><strong>MAE (Mean Absolute Error)</strong></li>
<li class="has-line-data" data-line-start="86" data-line-end="87"><strong>MSE (Mean Squared Error)</strong></li>
<li class="has-line-data" data-line-start="87" data-line-end="88"><strong>RMSE (Root Mean Squared Error)</strong></li>
<li class="has-line-data" data-line-start="88" data-line-end="89"><strong>AIC (Akaike Information Criterion) or BIC (Bayesian Information Criterion)</strong>: Information criteria that balance model complexity and goodness of fit. Lower values indicate better models.</li>
<li class="has-line-data" data-line-start="89" data-line-end="90"><strong>Ljung-Box Test</strong>: A statistical test to check if the residuals (forecast errors) are white noise, indicating a well-fitted model.</li>
<li class="has-line-data" data-line-start="90" data-line-end="92"><strong>Cross-Validation</strong>: Techniques like k-fold cross-validation or time series cross-validation assess a model’s performance on multiple test sets.</li>
</ul>
<h2 class="code-line" data-line-start=92 data-line-end=93 ><a id="Interpretation_of_Model_92"></a>Interpretation of Model</h2>
<ul>
<li class="has-line-data" data-line-start="94" data-line-end="96">Plot and check model outputs.</li>
</ul>
<h2 class="code-line" data-line-start=96 data-line-end=97 ><a id="Refinement_and_Improvement_96"></a>Refinement and Improvement</h2>
