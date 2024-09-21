EDA

Q) Compute summary statistics on a Spark DataFrame using .summary()?

A) spark_df.summary()


Q) Compute summary statistics on a Spark DataFrame using dbutils data summaries.

A)dbutils.data.summarize(df)

Q) Removeoutliers from a Spark DataFrame that are beyond or less than a designated threshold.

A) floor((p - err) * N) <= rank(x) <= ceil((p + err) * N).
   quantiles = df.approxQuantile("value", [0.25, 0.75], 0.01)
