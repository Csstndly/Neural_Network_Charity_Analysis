# Neural_Network_Charity_Analysis

## Analysis Purpose

The purpose of this analysis is to create a model that can predict 

## Results

### Data Preprocessing

The variable considered targets was the IS Successful Column.
 
The variables considered features for the model are the “Applicaltion_type”, “Affliation”, “Classification”, “Use_case”, “Organization”, “Special_Considerations”, “Ask_Amt” columns.

The variables that aren’t neither targets nor features are the EIN, Status, and Name column. They were removed as they didn’t give enough information about loan risk. EIN AND NAME were just numbers and names of the charities. The status column was removed as all rows but 5 were of the same status. 

### Compiling, Training, and Evaluating the Model

I selected 3 hidden layers to make the model more flexible so it’s less likely to overfit. The number of neurons were kept to a smaller amount as too many will have inverse effect of making the model worse (overfitting) or no effect at all. 

I was not able to achieve the target model performance. 

I took out the column “Status” as all but 5 were the same number so it wasn’t giving much information that I thought would affect the model. Tried to bin the “ASK_Amount” but it brought down the accuracy down so reverted it back to its original form. I ended up adding another hidden layer using the relu activation function and more neurons to the model. 

## Summary

The original model to the optimized model went from 57% accuracy to 58% accuracy. So, the increase wasn’t much. The loss metric stayed the same at 71%. I would recommend using a different activation function for one of the layers other than the relu function. Also trying to using a random forest as its pretty flexible and could improve accuracy. 
