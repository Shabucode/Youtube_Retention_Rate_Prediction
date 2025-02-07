

YouTube Video Retention Rate Prediction with Machine Learning Using Previous Data

Step 1: (Task 2)

Read the video scripts and the retention data for the training videos.

Segment the script based on the video position and create a dataset for predicting the retention rate with the following features:

Video position

Script segments

The dataset is saved in "full_retention_data_with_video_id.csv".

Video retention position timestamps are calculated based on the video length for 100 script segments.

Visualizations of "Retention Rate vs Script Segments" are showcased.

Step 2: (Task 2)

Convert the scripts into embeddings.

Train the model with the following features:

Script embeddings

Timestamp

"Compared to other videos (%)"

Predict the target variable: Retention rate.

Generate inferences for Video A after and before the first six timestamps.

Before inferencing for Video A, the script segments and their embeddings are generated.


Step 3: (Task 2)

Repeat Step 2 with the following features:

Script embeddings

Timestamp

Retention rates

Predict the target variable: "Compared to other videos (%)" for Video A after and before the first six timestamps.

The following file consists of the predictions of retention rate and "Compared to other videos (%)" for Video A with the original script:

"VIDEO_A_Predictions_Filled_Original_Script.csv"

Step 4: (Task 3)

Identify the intro segment from Video A.

Use an LLM to enhance the intro script.

Step 5: (Task 3)

Repeat Step 2 and Step 3 with the enhanced script.

The results are saved in the following file,

"Video_Predictions_filled_altered_intro.xlsx"

Drawbacks and Improvements Due to Time and Resource Constraints

State-of-the-art embeddings could be employed for better results.

As in Task 1, MLflow could be used for various model trials to select the best one.

Since one of the features is the script, which requires semantic understanding, advanced transformer models like BERT/DistilBERT could be employed for more accurate predictions.

Limited dataset: Results could be improved with more data samples. Few-shot learning could be used with advanced models, or LLMs could be fine-tuned with at least 30 samples.

The enhanced script did not show improved audience retention rates because the LLM is not fine-tuned for such tasks. To address this, an AI agent could be built using Langraph to enhance the intro hooks effectively.

The code complexity could be improved for better time and space efficiency.

Youtube Video Retention Rate Prediction with Machine Learning using Previous Data

Step 1: (Task 2)

Reading the video scripts and the retention data for the  training videos and segment the script based on the video position and create a dataset for predicting the retention rate with the features namely video position and script segments. The dataset is saved in "full_retention_data_with_video_id.csv".

Video retention position timestamp based on the video length for 100 script segments are calculated and the visualizations "Retention Rate vs Script Segments" are showcased.


Step 2: (Task 2)

The scripts are converted into embeddings and the model is trained with the following features, script embeddings, timestamp and "Compared to other videos (%)" and the target variable retntion rate is predicted. Inferences are made for Video A for after and before first 6 timestamps. Before inferencing for video A, the script segments and its embeddings are generated. 

The follwing file consits of the predictions of retention rate and Compared to other videos (%) for video A with the original script.
"VIDEO A_Predictions_Filled_Original_Script.csv"

Step 3: (Task 2)

Step 2 is repeated with the following features, script embeddings, timestamp and retention rates and the target variable, "Compared to other videos (%)" are predicted for Video A after and before first 6 timestamps.

Step 4: (Task 3)

The intro segment from the video A is identified and LLM is used to enhance the intro script.

Step 5: (Task 3)

Step 2 and 3 are repeated with the enhanced script and the results are filled in the file. 

The follwing file consits of the predictions of retention rate and Compared to other videos (%) for video A with the enhanced script.
"Video_Predictiions_filled_altered_intro.xlsx"

Drawbacks and Improvements due to time and resource contraints
1. State of art embeddings could be employed for better results.
2. As like task 1, MLflow could be employed for various model trials and better one could be selected.
3. As one of the features is script, which requires semantic understanding for predictions, advanced transformer models like BERT/distilBERT could be employed for more accurate predictions.
4. Limited Dataset. Results could be better with more data samples. Fewshot learning could be employed using advanced models or LLMs could be finetuned with the atleast 30 samples.
5. The enhanced script was not showcasing improved audience retention rates, that is due to the fact that the LLM is not finetuned for such tasks. To address that problem, an AI agent could be built using Langraph and which could be used to enhance the intro hooks.
6. The complexity of the code could be improved for time and space effiecieny.