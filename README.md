# YouTube Video Retention Rate Prediction with Machine Learning Using Previous Data

## Step 1: (Task 2)

- Reading the video scripts and retention data for the training videos.
- Segmenting the script based on the video position and creating a dataset for predicting the retention rate using the following features:
  - Video position
  - Script segments
- The dataset is saved in **"full_retention_data_with_video_id.csv"**.
- Calculating the video retention position timestamps based on the video length for 100 script segments.
- Visualizations,  **"Retention Rate vs Script Segments"** are showcased.

## Step 2: (Task 2)

- Converting the scripts into embeddings.
- Training the model using the following features:
  - Script embeddings
  - Timestamp
  - "Compared to other videos (%)"
- Predicting the **retention rate** as the target variable.
- Making inferences for **Video A** after and before the first six timestamps.
- Before inferencing for Video A, the script segments and their embeddings are generated.

## Step 3: (Task 2)

- Repeating Step 2 with the following features:
  - Script embeddings
  - Timestamp
  - Retention rates
- Predicting **"Compared to other videos (%)"** as the target variable for Video A after and before the first six timestamps.
- The following file contains predictions of retention rate and "Compared to other videos (%)" for Video A with the original script:
  - **"VIDEO_A_Predictions_Filled_Original_Script.csv"**

## Step 4: (Task 3)

- Identifying the **intro segment** from Video A.
- Using an **LLM** to enhance the intro script.

## Step 5: (Task 3)

- Repeating Steps 2 and 3 with the **enhanced script**.
- The results are saved in the following file:
  - **"Video_Predictions_filled_altered_intro.xlsx"**

## Drawbacks and Improvements Due to Time and Resource Constraints

1. **State-of-the-art embeddings** could be employed for better results.
2. Similar to **Task 1**, **MLflow** could be used to track various model trials and select the best one.
3. Since one of the features is **script text**, which requires **semantic understanding**, advanced transformer models like **BERT/DistilBERT** could improve predictions.
4. **Limited dataset**: Results could be improved with more data samples. **Few-shot learning** could be applied using advanced models, or **LLMs could be fine-tuned** with at least 30 samples.
5. The **enhanced script did not improve audience retention rates**, possibly because the **LLM is not fine-tuned for this specific task**. To address this, an **AI agent could be built using Langraph** to enhance intro hooks effectively.
6. The **code complexity** could be optimized for better **time and space efficiency**.
