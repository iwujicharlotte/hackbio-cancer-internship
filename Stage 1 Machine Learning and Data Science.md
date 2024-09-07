### **STAGE 1 MACHINE LEARNING AND DATA SCIENCE TASK**

### **(@Hackbio @slack @Charlotte @ChaimaBenMohamed @igwebuikevee0000 @Bonita)**

### **INTRODUCTION**

The article "**Multi-omic machine learning predictor of breast cancer therapy response" by Sammut *et al*., 2022** explores how integrating clinical, genomic, transcriptomic, and pathology data can enhance predictions of breast cancer treatment outcomes. The study involved 168 breast cancer patients treated with chemotherapy, with some receiving HER2-targeted therapy. By analyzing pre-treatment biopsies, the researchers examined tumor mutation burden, immune infiltration, and other features to assess their correlation with therapy responses, such as complete pathological response or residual disease.

### **METHODS**

The article highlights a machine learning framework developed to predict therapy responses in breast cancer. The model relies on a multi-step pipeline integrating multi-omic data, including genomic, transcriptomic, and clinical profiles. The training and external validation datasets were preprocessed and one hot encoded, followed by feature selection through univariable selection and collinearity reduction. The training data was fed to an unweighted ensemble classifier, combining predictions from three algorithms running in parallel: logistic regression, support vector machine (SVM), and random forest (RF). The final prediction was based on the average result from the three models. Hyperparameters optimization was performed using a five-fold cross-validation scheme. This involved splitting the data into five folds, training the model on four parts while testing on the remaining one. This process was repeated five times, with each fold serving as the test set once, ensuring the model generalized well. The model performance was fine-tuned and validated across different data splits, the fully integrated approach which combined clinical, DNA, RNA, digital pathology, and treatment data, achieved an AUC score of 0.87 on external validation. The model demonstrated a strong ability to predict pathological complete response (pCR), as evidenced by the ROC curve, which reflects the trade-off between sensitivity and specificity.

### **RESULTS AND DISCUSSION**

The findings indicated that the machine learning model integrating multi-omic data achieved a high predictive performance, with an AUC score of 0.87 in the external validation cohort. Based on the outcomes of this approach, the researchers demonstrated that treatment outcomes are modulated by the tumor ecosystem’s pre-treatment characteristics, such as immune activity and mutation profiles. For example, tumors with high mutation burdens and immune activation tended to respond better to therapy, particularly in HER2-negative cancers. Additionally, the study highlighted the role of clonal diversity and subclonal mutations in resistance to treatment, as these features were associated with residual disease. This integration of multi-omic data using machine learning demonstrated a high potential in aiding personalized therapy decisions for chemoresistant tumors by suggesting novel therapies when standard treatments may not be effective. The study revealed that tumor characteristics, including mutational burden, immune infiltration, and genetic mutations (like TP53 and PIK3CA), were critical in predicting responses to neoadjuvant therapy in breast cancer. The findings highlight the effectiveness of combining multi-omic data for better treatment personalization and improved outcomes.

### **SUMMARY**

This study highlights the importance of data integration in predictive models, advancing personalized medicine by providing more tailored treatment options based on the specific biological characteristics of each tumor.

### **REFERENCES**

Sammut, S. J., Crispin-Ortuzar, M., Chin, S. F., Provenzano, E., Bardwell, H. A., Ma, W., Cope, W., Dariush, A., Dawson, S. J., Abraham, J. E., Dunn, J., Hiller, L., Thomas, J., Cameron, D. A., Bartlett, J. M. S., Hayward, L., Pharoah, P. D., Markowetz, F., Rueda, O. M., Earl, H. M., … Caldas, C. (2022). Multi-omic machine learning predictor of breast cancer therapy response. *Nature*, *601*(7894), 623–629. https://doi.org/10.1038/s41586-021-04278-5