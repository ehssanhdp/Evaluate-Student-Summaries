# Student Summaries Evaluation Competition

## Goal of the Competition
The objective of this competition is to assess the quality of summaries written by students in grades 3-12. Participants are tasked with building a model that evaluates how well a student represents the main idea and details of a source text, along with assessing the clarity, precision, and fluency of the language used in the summary. The provided dataset includes real student summaries to train the model, and the outcome will aid teachers in evaluating student work quality while assisting learning platforms in offering immediate feedback to students.

## Dataset Description
The dataset consists of approximately 24,000 summaries composed by students in grades 3-12 across various topics and genres. Each summary is assigned scores for both content and wording. The competition's goal is to predict content and wording scores for summaries on unseen topics.

## File and Field Information
1. **summaries_train.csv:** Summaries in the training set.
   - **student_id:** ID of the student writer.
   - **prompt_id:** ID of the prompt linking to the prompt file.
   - **text:** The full text of the student's summary.
   - **content:** Content score for the summary (first target).
   - **wording:** Wording score for the summary (second target).

2. **summaries_test.csv:** Summaries in the test set, containing the same fields as the training set except for content and wording.

3. **prompts_train.csv:** Four training set prompts, each comprising the complete summarization assignment given to students.
   - **prompt_id:** ID linking to the summaries file.
   - **prompt_question:** Specific question students are asked to respond to.
   - **prompt_title:** Short-hand title for the prompt.
   - **prompt_text:** Full prompt text.

4. **prompts_test.csv:** Test set prompts, containing the same fields as the training set. Note that the prompts here are only an example, and the full test set has a large number of prompts. Train, public test, and private test splits do not share any prompts.

5. **sample_submission.csv:** A submission file in the correct format. Refer to the Evaluation page for details.

6. **Evaluate_Student_Summaries.ipynb:** jupyter notebook containg the code
   
Please note that this is a Code Competition. Example data is provided in `summaries_test.csv` and `prompts_test.csv` in the correct format. During scoring, this example test data will be replaced with the full test set, comprising about 17,000 summaries from numerous prompts.

